# Maintaining the public hub

## Repository boundary

Publish only curated documentation, selected public product assets and GitHub community configuration. Application source, packaging, signing, internal tests, workspace state, provider data and marketing contact lists belong outside this repository.

Never copy a private checkout or its Git history into this hub. Review the full staged file list before publication. Use explicit file paths when adding material and inspect images for private information.

## Organisation

- Keep the product introduction and entry points in the root README.
- Put public user guidance in `docs/` and update its README index.
- Put public images in `assets/`, with descriptive file names and attribution in its README.
- Put issue forms and community configuration in `.github/`; its organisation and coding-guideline rules are documented in [the configuration maintenance guide](../.github/maintenance.md).
- Keep rights, security reporting and contribution guidance at the root.

New maintained directories need a README describing their purpose, organisation and maintenance rules. Exception: use `maintenance.md` inside `.github/`, because GitHub gives `.github/README.md` precedence over the root product presentation. Keep the root README as the repository landing page. Avoid generic temporary or miscellaneous folders.

## Accuracy and guidelines

Distinguish shipped behaviour, beta limitations, illustrative screenshots and future proposals. Do not claim guaranteed correctness, security, provider endorsement, release dates or integrations without evidence.

**For code changes, use the project coding guidelines supplied by the maintainers.** For any future public sample, agree on its scope and license, keep it self-contained and apply appropriate checks before publishing. Application changes remain in the private repository under its full software and web guidelines.

## Validation

Check relative links and images, validate issue-form YAML, inspect diffs for private data, and verify the rendered README and issue chooser on GitHub. Documentation changes do not require an application build.
