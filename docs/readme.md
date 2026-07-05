# WinUI Developer Documentation

Welcome! This directory contains documentation for developers working *in* the WinUI repository.

> Looking for how to **use** WinUI in your own app? That documentation lives on
> [Microsoft Learn](https://learn.microsoft.com/windows/apps/winui/), not here.

## Getting started

- [Getting Started (build from GitHub)](../GettingStarted.md) - the concise, supported path to build WinUI from source. **Start here.**
- [Repo structure](repo-structure.md) - how the repository is laid out.
- [Developer guide](building/developer-guide.md) - the build in more depth, plus day-to-day tasks and advanced setup.
- [Contributing to WinUI](../CONTRIBUTING.md) - contribution process, PR requirements, and CLA.

## Building

- [Developer guide](building/developer-guide.md) - prerequisites, machine setup, and running a build.
- [Build system how-to](building/build-system-howto.md) - accomplishing common tasks with the build system.
- [Build system design](building/build-system-design.md) - how the build system is architected.
- [Advanced build topics](building/building-advanced.md)
- [Building sample apps](building/building-sample-apps.md)
- [Building a new-repo app](building/building-new-repo-app.md)
- [Controls developer guide](building/controls-developer-guide.md)
- [Submodules](building/submodules.md)
- [Common errors FAQ](common-errors-FAQ.md)
- [Ad-hoc testing of a local build with a fast inner loop](ad-hoc-testing-of-local-build-with-fast-inner-loop.md)

## Testing

- [Testing in WinUI FAQ](testing/testing-FAQ.md)
- [WinUI test system overview](testing/test-system-overview.md)
- [Test code in WinUI](testing/test-code-in-WinUI.md)
- [Testing baseline (image) files](testing/testing-baseline.md)
- [Testing with a C++ sample app](testing/testing-with-cpp-sample-app.md)
- [UAP tests](testing/uap-tests.md)
- [How to repro a XAML test failure](how-to-repro-a-xaml-test-failure.md)

## Debugging

- [Debugging](debugging/debugging.md)
- [Debugging tips](debugging/debugging-tips.md)

## Performance

- [Performance how-to](performance/perf-how-to.md)
- [ETW performance tracing](performance/perf-etw.md)
- [Profile-guided optimization (PGO)](performance/perf-pgo.md)

## Authoring & architecture

- [How to author a XAML control](how-to-author-a-xaml-control.md)
- [Design notes / code architecture](design-notes/readme.md) - high-level design docs and per-feature specs.
- [Property system](property-system.md)
- [Property path binding architecture](PropertyPathBindingArchitecture.md)
- [Hit testing](hit-testing.md)
- [Runtime-enabled features](runtime-enabled-features.md)
- [Telemetry events](telemetry-events.md)

## Publishing & release

- [Windows App SDK overview](winappsdk-overview.md) - how WinUI 3 integrates into the Windows App SDK.
- [Build pipelines](publishing/build-pipelines.md)
- [Build versioning](publishing/build-versioning.md)
- [Release channels](publishing/release-channels.md)
- [WinUI 3 release process](publishing/winui3-release-process.md)

## API specs & process

- [Public API review process](api-specs/public-api-review-process.md)
- [API review process](api-specs/api-review-process.md)
- Individual API specs live in [api-specs/](api-specs/).

## Contributing (external contributor docs)

- [Contribution handling](external/contribution_handling.md)
- [Contribution workflow](external/contribution_workflow.md)
- [Feature proposal process](external/feature_proposal_process.md)
- [Triage](external/triage.md)
- [Debugging build failures](external/debugging_buildfailures.md)
- [Debugging crashes](external/debugging_crashes.md)

## Writing docs

- [Documentation style guide](docs-style-guide.md)
- [Localization process](localization-process.md)

---

> Problem? Please file an issue for help.
>
> Found a bug? Please file an issue at [our issue tracker](https://github.com/microsoft/microsoft-ui-xaml/issues) and we'll triage it.