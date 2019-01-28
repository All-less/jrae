## Java Recursive Autoencoder

The original documentation can be found [here](https://github.com/sancha/jrae).


### Quick Start

```bash
gradle build  # compile source
gradle run  # launch main class 
```

Note that the program arguments (`application > run > args`) are defined in `build.gradle` and you may modify as you need.


### Caveats

The project depends on jblas, which requires several native libraries (especially `libs/{libjblas,libjblas_arch_flavor}.jnilib`). The location from where JVM will load them is defined in `build.gradle` (`application > applicationDefaultJvmArgs`) through `-Djava.library.path`. 

**Current settings are only tested on macOS.** If you are running on other platforms, please download jblas package from [here](https://github.com/downloads/mikiobraun/jblas/jblas-1.2.0.jar) , extract corresponding static libraries, place them as you like and set the library path accordingly.
