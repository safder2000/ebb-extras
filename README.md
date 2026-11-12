# Ebb Extras

Add-on for **Ebb**, the phone automation app. It adds features that Google Play doesn't allow in Ebb itself:

- **Record call**: record answered calls you choose (by SIM, contact or number)
- **App limits**: "used YouTube for 30 min today", "app opened", pause or close an app
- **Places**: run a flow when you arrive at or leave a place you draw on a map
- **Unlock guard**: run a flow after wrong PIN or pattern tries; lock or delete a folder

Ebb Extras has no flows of its own. Once installed, its blocks show up inside Ebb's editor and its results go to
Ebb's Activity. It only works with Ebb signed by the same developer.

## Download

Get the APK from [Releases](../../releases/latest).

## Install

1. Install **Ebb** (0.3.1 or newer) first. Android 12 or newer if your Ebb came from Google Play.
2. Download `ebb-extras-<version>.apk` on the phone and open it. Allow your browser or file manager to install apps
   if Android asks.
3. Open Ebb → **Setup**. An **Ebb Extras** section lists what each feature needs. Tap **Allow** on the ones you use.
4. **Android 13 and newer:** Android blocks the accessibility switch for apps installed from a file until you allow
   it. If the switch is greyed out: Settings → Apps → Ebb Extras → ⋮ (top right) → **Allow restricted settings**,
   then try again.

## Permissions

Each one is asked only when you tap Allow, with a short explanation first.

| Permission | Used for |
|---|---|
| Microphone + accessibility service | Record call (the accessibility service keeps the microphone during a call; it reads no screen content) |
| Phone state | Knowing when a recorded call ends |
| Usage access + accessibility service | App limits |
| Location, background location | Places |
| Device admin (watch login) | Unlock guard (counts wrong unlock tries only) |
| All files access | Lock or delete a folder |
| Notifications | The "recording" and "location in use" notices |
| Unrestricted battery | Keeping places and app limits working while the phone sleeps |

## Privacy

Ebb Extras has no internet permission. Recordings stay on your phone in `Recordings/Ebb`. Nothing is sent anywhere
unless one of your own Ebb flows sends it (for example a web request step you set up).

## Call recording and the law

Recording calls is restricted in some countries and states, and some require telling the other person. You are
responsible for using Record call legally. Quality: the other person is clear when the call is on speaker; on the
earpiece it depends on the phone.

## Verify the download

Signing certificate SHA-256:
`97:C8:3A:02:F8:46:66:A6:E7:02:BC:24:97:3F:C3:9C:51:C4:38:0A:FF:8C:1D:B1:EC:F3:55:97:86:9F:80:AF`
