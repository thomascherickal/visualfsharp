# The F# language, Core library, and F# tools for Visual Studio

You're invited to contribute to future releases of the F# language compiler, core library, and tools. Development of this repository can be done anywhere [.NET Core](https://dotnet.microsoft.com/) is supported: Windows, macOS, and a variety of Linux distributions.

## Contributing

### Quickstart on Windows

Build from the command line:

```bash
build.cmd
```

You can then open either `FSharp.sln` or `VisualFSharp.sln` in your editor of choice. The latter solution is larger but includes the F# tools for Visual Studio and its associated infrastructure.

### Quickstart on Linux or macOS

Build from the command line:

```bash
sh ./build.sh
```

You can then open `FSharp.sln` in your editor of choice.

### More options and information

See [DEVGUIDE.md](DEVGUIDE.md) and [TESTGUIDE.md](TESTGUIDE.md) for more details on additional configurations for building and testing, how to update compiler error messages, and more.

## Build Status

| Branch | Status |
|:------:|:------:|
|master|[![Build Status](https://dnceng.visualstudio.com/_apis/public/build/definitions/9ee6d478-d288-47f7-aacc-f6e6d082ae6d/106/badge?branchname=master)](https://dnceng.visualstudio.com/public/public%20Team/_build?definitionId=106&_a=history)|
|dev15.9|[![Build Status](https://dnceng.visualstudio.com/_apis/public/build/definitions/9ee6d478-d288-47f7-aacc-f6e6d082ae6d/106/badge?branchname=dev15.9)](https://dnceng.visualstudio.com/public/public%20Team/_build?definitionId=106&_a=history)|
|dev16.0|[![Build Status](https://dnceng.visualstudio.com/_apis/public/build/definitions/9ee6d478-d288-47f7-aacc-f6e6d082ae6d/106/badge?branchname=dev16.0)](https://dnceng.visualstudio.com/public/public%20Team/_build?definitionId=106&_a=history)|

## Using nightly releases in Visual Studio

You can use the latest `master` build of the F# compiler and tools for Visual Studio via our nightly releases if you are a Visual Studio users. See details on setup here:

https://blogs.msdn.microsoft.com/dotnet/2017/03/14/announcing-nightly-releases-for-the-visual-f-tools/

### Even more nightly than the nightly

Alternatively, if you _really_ want to live on the bleeding edge, you can set up a nightly feed for the Visual Studio preview releases, which use the latest commit in the preview branch of this repository. To do so, follow the same instructions as the above blog post, but instead with these links:

* Set your feed to the [preview feed](https://dotnet.myget.org/F/fsharp-preview/vsix)
* Install manually from the [preview feed](https://dotnet.myget.org/feed/fsharp-preview/package/vsix/VisualFSharp)

## Branches

These are the branches in use:

* `master`
  - Most contributions go here.
  - Able to be built, installed and used in the latest public Visual Studio release.
  - May contain updated F# features and logic.
  - Used to build nightly VSIX (see above).
  - Gets integrated into https://github.com/fsharp/fsharp to form the basis of Mono releases
  - Gets integrated into https://github.com/fsharp/FSharp.Compiler.Service to form the basis of FSharp.Compiler.Service releases

* `dev15.9`
  - Long-term servicing branch for VS 2017 update 15.9.x. We do not expect to service that release, but if we do, that's where the changes will go.
  
* `dev16.x`
  - Latest release branch for the particular point release of Visual Studio.
  - Incorporates features and fixes from master up to a particular branch point, then selective cherry-picks.
  - May contain new features that depend on new things or fixes in the corresponding forthcoming Visual Studio release.
  - Gets integrated back into master once the corresponding Visual Studio release is made.

## F# language and core library evolution

Evolution of the F# language and core library follows a process spanning two additional repositories. The process is as follows:

1. Use the [F# language suggestions repo](https://github.com/fsharp/fslang-suggestions/) to search for ideas, vote on ones you like, submit new ideas, and discuss details with the F# community.
2. Ideas that are "approved in principle" are eligible for a new RFC in the [F# language design repo](https://github.com/fsharp/fslang-design). This is where the technical specification and discussion of approved suggestions go.
3. Implementations and testing of an RFC are submitted to this repository.

## Additional project documentation

The following links can help you get an overview of some technical aspects of the F# language and compiler:

* [The F# Compiler Technical Guide](http://fsharp.github.io/2015/09/29/fsharp-compiler-guide.html) 
* [The F# Language Specification](http://fsharp.org/specs/language-spec/)

## License

This project is subject to the MIT License. A copy of this license is in [License.txt](License.txt).

## Code of Conduct

This project has adopts the [Contributor Covenant](http://contributor-covenant.org/) code of conduct to clarify expected behavior in our community. You can read it at [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md).

## Get In Touch

Members of the [F# Software Foundation](http://fsharp.org) are invited to the [FSSF Slack](http://fsharp.org/guides/slack/). The `#compiler` and `#editor-support` channels are where other contributors typically chat with others.

Additionally, you can use the `#fsharp` tag on Twitter if you have general F# questions, including about this repository. Chances are you'll get multiple responses.

## About F#

If you're curious about F# itself, check out these links:

* [What is F#](https://docs.microsoft.com/dotnet/fsharp/what-is-fsharp)
* [Get started with F#](https://docs.microsoft.com/dotnet/fsharp/get-started/)
* [F# Software Foundation](http://fsharp.org)
* [F# Testimonials](http://fsharp.org/testimonials)
