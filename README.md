# Winepak
Flatpak-ing Microsoft Windows applications with Wine.

## Goals
* Package `wine` applications via `flatpak`
* Make installing and running applications Just Work<sup>TM</sup>

## Repos
* [winepak-sdk-images](https://github.com/winepak/winepak-sdk-images): The Sdk & Platform for `winepak`
* [applications](https://github.com/winepak/applications): A collection of flatpak manifest for building Microsoft Windows applications via `winepak`

## Instructions
To get started with winepak you first need to build & install the Sdk & Platform, instructions can be found on the [winepak-sdk-images](https://github.com/winepak/winepak-sdk-images) repo.

Next pick an application to build & install. A list of them with instructions can be found in the [applications](https://github.com/winepak/applications) repo. Take note of the Platform branch the application uses. Most games require the `staging` branch of Sdk/Platform.

## Note
Winepak currently lacks WoW64 support in the 64bit version of `wine`. Without WoW64 most windows applications won't install and/or run. Many 64bit applications in Windows link to 32bit libraries and need the syswow64/WoW64 capability layer. This is being addressed in [flatpak-builder 10.10](https://github.com/flatpak/flatpak-builder/releases/tag/0.10.10).
