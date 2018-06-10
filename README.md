# Winepak
Flatpak-ing Microsoft Windows applications with Wine.

## Goals
* Package `wine` applications via `flatpak`
* Make installing and running applications Just Work<sup>TM</sup>

## Repos
* [winepak-sdk-images](https://github.com/winepak/winepak-sdk-images): The Sdk & Platform for `winepak`
* [applications](https://github.com/winepak/applications): A collection of flatpak manifest for building Microsoft Windows applications via `winepak`

## Instructions
See [winepak.org](https://www.winepak.org) for instructions using the remote repo.

### Building
To get started with winepak you first need to build & install the Sdk & Platform, instructions can be found on the [winepak-sdk-images](https://github.com/winepak/winepak-sdk-images) repo.

Next pick an application to build & install. A list of them with instructions can be found in the [applications](https://github.com/winepak/applications) repo. Take note of the Platform branch the application uses. Most games require the `staging` branch of Sdk/Platform.
