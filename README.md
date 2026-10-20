# Serenity Home: Windows .exe and Android .apk

## Get the installers (no build tools needed on your computer)
1. Create a free account at github.com and make a new empty repository.
2. Upload everything in this folder to it, including the hidden .github folder.
3. Open the repo, click Actions, choose "Build Serenity Home", click Run workflow.
4. After about 10 minutes, open the finished run. Under Artifacts, download:
   - SerenityHome-Windows-exe (the .exe installer and portable app)
   - SerenityHome-Android-apk (the .apk; on the phone allow "install unknown apps")

## Google Drive storage (rinenroy@gmail.com)
Not switched on yet. It needs your own Google Cloud OAuth client ID, which only
you can create while signed in as rinenroy@gmail.com:
1. console.cloud.google.com: create a project and enable the Google Drive API.
2. Create an OAuth client ID (Web for Windows, Android for the phone).
3. Send the client ID to Claude and the Drive sync code will be added.
Google blocks sign-in inside plain embedded web views, so Windows will use the
system browser and Android will use Google's native sign-in plugin.

## Notes
- The apps contain Serenity Home and open the three sites inside it. Some sites
  may refuse to be embedded; the "Open in new tab" button handles that.
- Debug APKs are fine for personal use. A Play Store release needs signing.
