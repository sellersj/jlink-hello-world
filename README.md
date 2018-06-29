# jlink-hello-world

This is a test application for making a "jre included" jar.
It requires a maven toolchain configured with a jdk 10.

All modules need a module-info.java file or you'll get an error like
"Error: automatic module cannot be used with jlink"
