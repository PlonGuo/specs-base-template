# Specs Base Template

A Lens Studio project for Spectacles, starting from the Specs Base Template.

## Open the project

1. Install Lens Studio 5.24.1 (the version recorded in the project manifest).
2. Open `Specs Base Template.esproj`.
3. Allow Lens Studio to import the assets and packages and regenerate its local caches.

## Repository contents

- `Assets/`: the scene, render resources, and asset metadata.
- `Packages/`: Spectacles Interaction Kit and Spectacles UI Kit packages, with their metadata.
- `Specs Base Template.esproj`: the Lens Studio project manifest.
- `AGENTS.md` and `CLAUDE.md`: project guidance for coding agents.
- `skills-lock.json`: the source and content hash of the optional `plan-lens` skill.

Generated caches, generated API definitions, local editor state, machine-specific MCP configuration, and downloaded skill copies are excluded from version control.

## Optional planning skill

To restore the `plan-lens` skill from `challengepost/learn-specs`, run this from the project folder with Node.js 22.20.0 or newer:

```sh
npx --yes skills@1.7.4 add challengepost/learn-specs --all -y
```

The skill helps prepare a Lens design brief before implementation. The command downloads the current upstream skill; `skills-lock.json` records the version installed for this snapshot.

## License

Project-authored contributions are licensed under the [MIT License](LICENSE).
Bundled Lens Studio template assets and Spectacles packages remain subject to their upstream terms; any embedded copyright and license notices are preserved.
