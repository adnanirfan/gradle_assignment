# Gradle Multi Module Project (Assignment)

## Task: 
Instructions
You are assigned to build a complete multi module zip file which will contain a zip file for each module.
You need to create three tasks in total.

1. Download project from slack channel.
2. Extract the zip file.
3. Try building it with `./gradlew -i build`
3.1. If it does not build, tell us the error you are facing.
4. Create two tasks for `node-module`.
4.1. Create a task which cleans `node_module` and `package-lock.json` files in `node-module` project.
4.1.1. Assign  `node-module`'s `clean` dependency on this task.
4.2. Create a task which creates a zip archive of complete `node-module` project.
4.2.1. You need to exclude files which are not necessary for production build (`node_modules` is part of your build).
HINT: Development Environment Files.
4.2.2. Assign `node-module`'s `assemble` dependency on this task.
5. Create a task for root project.
5.1. Create a task which creates a zip archive of each module's build archive.
5.1.1. Example: `java-module` creates its zip archive inside `java-module/build/libs`, `node-module` will create in `node-module/build/distributions`.
6. Create task dependency such that root project's task run in last.
7. Copy tasks that you made in a text file separated by module name along with task dependency assignment `and submit it.

Helping material: https://docs.gradle.org/current/userguide/working_with_files.html

### Commands 
1. `./gradlew -m build` // to check tasks sequence
1. `./gradlew clean` // clean builds

