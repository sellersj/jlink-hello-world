# jlink-hello-world

## Required things needed
This is a test application for making a "jre included" jar.
It requires a maven toolchain configured with a jdk 10.

## How to run the code and expected output
Need to checkout plugin from source and run `mvn install -DskipTests`
https://github.com/apache/maven-jlink-plugin

`mvn package`
This will create a zip under the `jlink-hello-world-jlink/target`
If you unzip this file, you can run the code like this which will use the packaged jre
`bin/launch`

Expected output
```
$ bin/launch
Hello world, java version is: 10.0.1
```

## Trouble shooting
All modules need a module-info.java file or you'll get an error like
"Error: automatic module cannot be used with jlink"

## Notes
Another example that would have been useful to find is
https://github.com/khmarbaise/jdk9-jlink-jmod-example/tree/master/maven-example
