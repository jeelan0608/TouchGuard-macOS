# TouchGuard for macOS

TouchGuard asks macOS to authenticate with Touch ID (or your Mac password) when you open selected apps. The free plan protects one app; Pro adds unlimited protected apps and schedules for three months per purchase.

## Download and install

1. Download `TouchGuard-macOS.zip` from the latest GitHub Release and unzip it.
2. Keep `TouchGuard.app` and `Install-TouchGuard-Background.command` together. Move both to your Applications folder.
3. Open TouchGuard. If macOS says it cannot verify the developer, Control-click the app, choose **Open**, then confirm.
4. Open the installer command file and allow Terminal to run it. It installs the background helper for your user and starts protection at login.
5. In TouchGuard, select the apps you want to protect and turn protection on.

TouchGuard requires macOS 13 or newer and a Mac account with Touch ID configured. macOS may offer your account password as a fallback.

## Notes

- TouchGuard uses macOS LocalAuthentication for the system authentication prompt.
- macOS does not provide ordinary apps with a supported way to block another app before it launches. A protected app may briefly appear before TouchGuard closes it and requests authentication.
- This download is not notarized by Apple. The first launch may require the Control-click → Open step above.
- Pro activation is currently handled manually after payment. A purchase does not automatically activate until a valid activation code is entered.

## Source

Download `TouchGuard-Source.zip` for the Swift source and Swift Package manifest. The prebuilt app bundle is provided in the release ZIP for convenience.
