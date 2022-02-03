# showkase-screenshot-tests

Sample app for integration between Showkase library and Facebook's screenshot testing library

./gradlew runDebugAndroidTestScreenshotTest

creates a nice HTML report with all your composable screenshots. This is useful mainly when you are
developing or maintaining tests — you can see them at one place.

./gradlew recordDebugAndroidTestScreenshotTest

saves all screenshot image files to a folder. You can push these images into git and create (or
update) your “golden” screenshots.

./gradle verifyDebugAndroidTestScreenshotTest

compares your “golden” screenshots created by previous command with the latest ones. If fails the
build if there are some differences in the images.