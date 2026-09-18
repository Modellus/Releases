# Modellus downloads

The desktop installers for Modellus, and nothing else.

- macOS: [Modellus-mac.dmg](https://github.com/Modellus/Releases/releases/latest/download/Modellus-mac.dmg)
- Windows: [Modellus-windows.exe](https://github.com/Modellus/Releases/releases/latest/download/Modellus-windows.exe)

The application itself is built from `Modellus/EditorHtml`, which is private. This repository is
public so that anyone can download the installers without a GitHub account, and so that the macOS and
Windows runners that build them cost nothing.

The build here checks the application out with a read-only deploy key and publishes the result as the
`latest` release. It runs when someone starts it from the Actions tab, and once a day, and on that
daily run it builds only if the application's `main` has moved since the release was last made.
