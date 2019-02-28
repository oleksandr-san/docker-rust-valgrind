# docker-rust-valgrind
Docker image containing rust and valgrind.

Usefull for MacOS which reqularly release kernel version that is higher than supported version for Valgrind. You can get around this problem by running valgrind in container. E.g.
```
docker run -v  `pwd`:/js -it retep007/rust-valgrind bash
```

Common error message when installing Valgrind on unsupported MacOS is
```
valgrind: This formula either does not compile or function as expected on macOS
 versions newer than Sierra due to an upstream incompatibility.
```
