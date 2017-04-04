## Avalitan's CA Module for [Magisk](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445 "Magisk Thread on XDA")
This is my CA module for Magisk, you can also download it from my [page](http://ca.avalitan.com/?os=a)




## Best Practice for Updating a Repo
1. Open a new branch, and start update your files on the new branch
2. Test if everything works fine
3. Bump up the `versionCode` in `module.prop`, or Magisk Manager won't know that your module is updated!
4. Merge the changes back to master, all users shall now receive the update in Magisk Manager

## Notes
1. (Windows aware!!) This git repo is configured to force Unix endlines on all necessary files. The line endings on these files should remain the Unix format. Please use advanced text editors like Sublime, Atom, Notepad++ etc. to edit the text files
2. In `module.prop`, `version` is any string you like, so any fancy version name (e.g. ultra-beta-v0.0.0.1) is allowed. However, `versionCode` **MUST** be an integer. The value is used for version comparison.
2. Make sure your module ID **doesn't contain any spaces**.
3. (For repo developers) Magisk Manager monitors all repo's `master` branch. So any changes to the branch `master` will be reflected to all users immediately. If you are working on an update for a module, please work on another branch, make sure it works, and then merge the changes back to `master`.
