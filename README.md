# OUDS Web Skills

[Agent skills](https://skills.sh) for building interfaces with [OUDS Web](https://github.com/Orange-OpenSource/Orange-Boosted-Bootstrap/), the web implementation of the Orange Unified Design System.

Once installed, your AI coding agent knows the OUDS Web components, layout, utilities and design tokens, and can migrate existing projects to OUDS Web.

## Available skills

| Skill | Description | Applies to |
| --- | --- | --- |
| [`using-ouds-web-1.5`](./using-ouds-web-1.5) | Reference for OUDS Web: components, layout, utilities, foundation (typography, color modes, CSS variables, Sass), getting started. | OUDS Web **1.5.x** |
| [`migrate-to-ouds-web`](./migrate-to-ouds-web) | Guided migration from OB1, Boosted or an older OUDS Web version, using the `@ouds/web-migrate` CLI. | Any source version |

## Installation

```bash
npx skills add Orange-OpenSource/ouds-web-skills
```

The command is interactive and lets you choose which skills to install.

## Versioning

The `using-ouds-web-<version>` skill is tied to a specific version of the OUDS Web library, indicated by the suffix in its name (e.g. `1.5` for OUDS Web 1.5.x).

A new skill folder is generated in this repository at each release of the library.

> [!IMPORTANT]
> Whenever you update OUDS Web in your project, update the skill too: run `npx skills add Orange-OpenSource/ouds-web-skills` again and use the skill matching your new library version. Remove the previous versioned skill to avoid conflicting guidance.

## Repository structure

```text
.
├── migrate-to-ouds-web/
│   └── SKILL.md
└── using-ouds-web-1.5/
    ├── SKILL.md
    └── references/
        ├── components/
        ├── foundation/
        ├── getting-started/
        ├── layout/
        └── ...
```

## Contributing

The content of this repository is **generated at each release** of OUDS Web. Do not edit it here: changes would be overwritten.

The sources of the skills live in the library repository. To report an issue or propose a change, please contribute there: [Orange-OpenSource/Orange-Boosted-Bootstrap](https://github.com/Orange-OpenSource/Orange-Boosted-Bootstrap/).

## License

Released under the [MIT License](./LICENSE).
