## KoT (Knowledge of Things)

*Knowledge from Earth to Universe.*

KoT helps you define and coordinate a verifiable, provenance-aware knowledge continuity framework for "things" (entities, systems, and phenomena). It does this by providing a document-first charter, scope, glossary, and proposal process so that you can align stakeholders and build interoperable specifications over time.

Project status: early-stage (document-first, no code yet)

### Basic functionality

KoT is intended for use by standards bodies, knowledge communities, researchers, and builders across relevant ecosystems. It is meant to help these stakeholders do the following:

* Align on terminology and scope boundaries
* Document use cases, risks, and stakeholder needs
* Propose and review changes transparently
* Converge on draft specifications (later)

KoT uses public documentation and a lightweight proposal workflow to do this. It takes stakeholder requirements and ecosystem references from contributors and uses them to refine KoT's charter, scope, principles, and glossary. For more details about the repository structure and tooling, see the [developer documentation](#developer-documentation).

### What KoT does not do

KoT is not intended to replace existing knowledge bases or communities. It is a coordination and standardization effort.

Later phases may include specifications, reference implementations, and pilot deployments, but they are out of scope for the current stage.

## Prerequisites

Before using KoT, you should be familiar with:

* The basics of knowledge graphs and linked data
* The basics of provenance and integrity concepts
* How to use GitHub issues and pull requests

You should have:

* A GitHub account (to participate in issues, proposals, and pull requests)
* Node.js and npm (optional, for running Markdown linting and formatting)

## How to use KoT

### Read the charter and scope

1. Read [`CHARTER.md`](./CHARTER.md).
   1. Note the mission and vision.
   2. Note the in-scope and out-of-scope boundaries.
2. Read [`docs/scope.md`](./docs/scope.md).
3. If anything is unclear, open an issue with questions or suggested edits.

### Propose a change

1. Decide whether the change is small or significant.
   1. For small edits, open a pull request.
   2. For significant changes, follow the proposal process.
2. Read [`proposals/README.md`](./proposals/README.md).
3. Open an issue describing the proposal and motivation.
4. After discussion, open a pull request that updates the relevant documents.

### Add a use case or reference

1. Read [`docs/use-cases.md`](./docs/use-cases.md) and [`docs/references.md`](./docs/references.md).
2. Add a concise use case or reference.
   1. Keep scope in mind (see [`docs/scope.md`](./docs/scope.md)).
   2. Use neutral, verifiable language.
3. Open a pull request.

### Run Markdown checks (optional)

1. Install dependencies.
   1. Run `npm install`.
2. Check Markdown.
   1. Run `npm run lint:md`.
3. Apply automatic formatting.
   1. Run `npm run format:md`.

## Troubleshooting

Markdown linting fails

* Run `npm run format:md` and try again.

Not sure whether a change needs a proposal

* Start with [`proposals/README.md`](./proposals/README.md). If the change affects charter, scope, or governance, open an issue first.

## How to get help and report issues

* Report issues at https://github.com/doguabaris/kot/issues.
* Ask questions by opening an issue and using a "question" label. Response time is best effort.

## Developer documentation

### Technical implementation

KoT is currently document-first. The repository uses Markdown for documents and `remark` for linting and formatting.

### Code structure

* `docs/` contains the vision, scope, principles, glossary, FAQs, and supporting material.
* `proposals/` contains the proposal process and future proposal drafts.
* Root documents ([`CHARTER.md`](./CHARTER.md), [`GOVERNANCE.md`](./GOVERNANCE.md), [`ROADMAP.md`](./ROADMAP.md)) define KoT's initiative boundaries and process.

### Local development

#### Set up

How to set up a local environment:

1. Install Node.js (LTS) and npm.
2. Clone the repository.

#### Install

How to install dependencies:

1. Run `npm install`.

#### Configure

No configuration is required for the document-only phase.

#### Build and test

There is no build step yet. To run Markdown checks:

1. Run `npm run lint:md`.

To apply formatting:

1. Run `npm run format:md`.

#### Debugging

* `remark` exits with warnings or errors
  * Fix the reported Markdown issues, then rerun `npm run lint:md`.

## How to contribute

The KoT maintainers welcome contributions.

* Clarify scope, definitions, and non-goals
* Add references and cross-ecosystem mapping notes
* Write or review proposals

### Contribution process

Before contributing, read [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md) to understand community guidelines and expectations. We follow https://developer.mozilla.org/en-US/docs/MDN/Writing\_guidelines/Writing\_style\_guide for writing style.

1. Open an issue describing the change.
   1. For proposals, follow [`proposals/README.md`](./proposals/README.md).
2. Open a pull request with a focused change.
3. Participate in review and discussion.

## Credits

KoT is led by Doğu Abaris and built with contributions from the community.

## License

KoT is under the MIT License. See [`LICENSE`](./LICENSE) for details.
