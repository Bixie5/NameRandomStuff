# Random Picture app

1. Create a new GitHub repo and upload everything in this folder (keep the `.github` folder).
2. Open the **Actions** tab. The "Build APK" workflow runs on every push to main/master, or click **Run workflow**.
3. When it finishes, open the run and download the `random-picture-apk` artifact (a zip containing `app-debug.apk`).
4. Unzip, copy the APK to your phone and install it (allow "install unknown apps").

## Updating the app / making deletions permanent
- Edit `www/index.html` and push; Actions rebuilds the APK.
- To bake deletions into the APK: in the browser version, delete entries, click "save permanent copy", then replace `www/index.html` with the downloaded file and push.
- Inside the APK, deletions are remembered on that phone, but "save permanent copy" may not download there. Use the browser version for that.
