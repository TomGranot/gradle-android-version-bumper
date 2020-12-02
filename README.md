# gradle-version-bumper

While writing [this article](https://granot.dev/continuous-integration-deployment-for-android-using-circleci-top-to-bottom-tutorial/) I needed to write a small bash script that bumps an Android app's version number in the following way:

If `version=XXX.YYY.ZZZ`, do `version=XXX.(YYY + 1).(ZZZ + 20)`

And edit the app's `app/build.gradle` file.

# Installation
If you've got a standard Android project, go to the folder and then do:

```shell
mkdir scripts
cd scripts
```

Then drop the file in there, and when you're done:

```shell
cd ..
chmod 777 -R scripts
```
To ensure the CI server won't cause you problems.

**Note:** This works as a standalone script, but you probably should read the article above for context.
