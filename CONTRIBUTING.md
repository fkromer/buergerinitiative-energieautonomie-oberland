# Contributing

## Dev Setup

- [install](https://www.jetify.com/docs/devbox/installing_devbox/#install-devbox) [devbox](https://www.jetify.com/devbox)
- `devbox shell`
- `npx astro dev`
- http://localhost:4321
- happy coding 🙂

## Branch Strategy

- `buergerinitiative-energieautonomie-oberland:website`
  - Is forked from [`astrogon/astrogon:main`](https://github.com/astrogon/astrogon/tree/main).
  - Results in deployed
    [buergerinitiative-energieautonomie-oberland.de](https://buergerinitiative-energieautonomie-oberland.de/)
    website.
- `buergerinitiative-energieautonomie-oberland:<contribution>`
  - Code base which extends
  `buergerinitiative-energieautonomie-oberland:website` with contribution.
  - Is live previewed in PRs like e.g. [in this PR](https://github.com/fkromer/buergerinitiative-energieautonomie-oberland/pull/1).

## Branch Workflows

### Contributor Workflows

- `git clone git@github.com:fkromer/buergerinitiative-energieautonomie-oberland.git`
- `git checkout website`
- `git checkout -b <contribution>`
  - Contribution of a new/change of an existing/removal of a deprecated network participant==
    [author](https://buergerinitiative-energieautonomie-oberland.de/authors/)==
    [person responsible for journalistic content](https://buergerinitiative-energieautonomie-oberland.de/terms/): `<contribution>` ➡️ `network-<something>`
    - Removal of a deprecated network participant implies the need for changing the
      [author](https://buergerinitiative-energieautonomie-oberland.de/authors/)==
      [person responsible for journalistic content](https://buergerinitiative-energieautonomie-oberland.de/terms/)
      to another author beforehand or the removal of all blog posts created by this author.
  - Contribution of a new/change of an existing/removal of an existing blog post (author must exist beforehand): `<contribution>` ➡️ `blog-post-<something>` important
  is that it's based on the `website` branch)
- edit (add/change/remove) code
- `git commit`
- `git push origin <contribution>`
- create PR
- iterative code edit, `git commit`, PR review loop until ready to merge
- (PR is merged using squash merging automatically.)

## Deployments (maintainer/ownder only)

[Netlify Project](https://app.netlify.com/projects/buergerinitiative-energieautonomie/overview)
