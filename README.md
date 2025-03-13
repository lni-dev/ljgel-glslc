# GlslC

This plugin simply calls glslc from gradle to compile shaders to binary during your gradle build.
`glslc` must be installed and in the `PATH` environment variable.

## Apply Plugin
```groovy
plugins {
    id 'de.linusdev.ljgel.glslc' version '+'
}
```

## Use
```groovy
glslc {
    shaderLocation = '/src/main/glsl/shaders' // The path where your .vert and .frag files are located
    compiledShadersRootResourcesPackage = 'shaders' // The java resource folder, where the compiled shaders will be stored
}
```