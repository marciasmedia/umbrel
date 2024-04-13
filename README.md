
Skip to content

    marciasmedia
    /
    umbrell-app

Code
Issues
Pull requests
Projects
Security
Insights

    Settings

Commit
Add files via upload

    main 

@marciaskosz
marciaskosz committed Apr 6, 2024
0 parents commit d074338
Showing 3 changed files with 42 additions and 0 deletions.

1 change: 1 addition & 0 deletions 1
.gitignore
@@ -0,0 +1 @@
.DS_Store
39 changes: 39 additions & 0 deletions 39
README.md
@@ -0,0 +1,39 @@
## Umbrel Community App Store Template

This repository is a template to create an Umbrel Community App Store. These additional app stores allow developers to distribute applications without submitting to the [Official Umbrel App Store](https://github.com/getumbrel/umbrel-apps).

Just click the "Use this template" button above and start adding your own apps!

### Technical Details

The `umbrel-app-store.yml` file defines two important properties:
- `id` - This is used as a prefix for all apps within the community app store. You **MUST** prefix your application id with your app store ID. For example, this template defines `sparkles` as a community app store ID and we have a `hello world` app. The app ID therefore should be: `sparkles-hello-world`
- `name` - This name appears within the Umbrel user interface when users explore apps within these community app stores.


### Testing

To test your community app store, you can add this repository through the Umbrel user interface as shown in the following demo:


https://user-images.githubusercontent.com/10330103/197889452-e5cd7e96-3233-4a09-b475-94b754adc7a3.mp4


Alternatively, you can use the Umbrel CLI as described below.

To add an app store:
```
sudo ~/umbrel/scripts/repo add https://github.com/getumbrel/umbrel-community-app-store.git
sudo ~/umbrel/scripts/repo update
```

To install an app from the app store
```
sudo ~/umbrel/scripts/app install sparkles-hello-world
```

To remove an app store:
```
sudo ~/umbrel/scripts/repo remove https://github.com/getumbrel/umbrel-community-app-store.git
```
2 changes: 2 additions & 0 deletions 2
umbrel-app-store.yml
@@ -0,0 +1,2 @@
id: "sparkles" # Choose the ID for your app store. This should contain only alphabets ("a to z") and dashes ("-").
name: "Sparkles" # Choose the name of your app store. It will show up in the UI as "<name> App Store".
0 comments on commit d074338
@marciasmedia
Comment

Leave a comment
Footer
© 2024 GitHub, Inc.
Footer navigation

    Terms
    Privacy
    Security
    Status
    Docs
    Contact

Add files via upload · marciasmedia/umbrell-app@d074338
