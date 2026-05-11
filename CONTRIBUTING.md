# Contributing

Thanks for helping keep the Elyan Labs profile repository accurate and useful. This repo is the public profile for `Scottcjn`, so changes should be small, factual, and easy to verify.

## Repository Scope

- `README.md` is the GitHub profile README and should stay focused on current projects, merged work, and active areas of focus.
- `external-pr-portfolio.md` tracks external upstream pull requests and should only include public, verifiable PRs.
- Keep additions aligned with Elyan Labs work: RustChain, BoTTube, Beacon, vintage hardware, portability, performance, and ecosystem documentation.

## Before You Open a Pull Request

1. Pull the latest `main` branch and create a topic branch for your edit.
2. Keep the diff narrow. Avoid unrelated wording, formatting, or ordering changes.
3. Verify every new claim with a public link, such as a merged PR, project page, accepted paper, or repository.
4. Preview Markdown locally or in GitHub to catch broken tables, headings, and relative links.
5. Run a spelling pass on edited Markdown when possible:

   ```sh
   codespell README.md external-pr-portfolio.md CONTRIBUTING.md
   ```

## Profile README Guidelines

- Keep the first screen concise and current.
- Prefer specific project links over broad claims.
- Update star counts, merged PR counts, dates, and status labels only when the public source supports the change.
- Do not add private contact details, unpublished claims, or unverifiable metrics.

## External PR Portfolio Guidelines

- Add only public external PRs authored by `Scottcjn`.
- Place new merged PRs under the correct month and keep table rows sorted by merge date, newest first.
- Move a pending PR into the merged section only after GitHub shows it as merged.
- Include enough context for readers to understand why the upstream contribution matters, but keep descriptions brief.

## Pull Request Checklist

- The change is limited to profile documentation.
- New links resolve and point to the intended source.
- Tables still render correctly.
- Counts, dates, and status labels match the linked evidence.
- The PR description explains what changed and why.
