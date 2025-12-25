# linmath.h

<h6>A small library for linear math as required for computer graphics</h6>

<!-- [![CircleCI](https://circleci.com/gh/datenwolf/linmath.h.svg?style=svg)](https://app.circleci.com/pipelines/github/datenwolf/linmath.h) -->

linmath.h provides the most used types required for programming computer graphics:

- `vec3` -- 3 element vector of floats
- `vec4` -- 4 element vector of floats (4th component used for homogenous computations)
- `mat4x4` -- 4 by 4 elements matrix, computations are done in column major order
- `quat` -- quaternion

The types are deliberately named like the types in GLSL. In fact they are meant to
be used for the client side computations and passing to same typed GLSL uniforms.

<br>

## Installation

Run:

```sh
$ npm i linmath.c
```

And then include `linmath.h` as follows:

```c
// main.c
#include "node_modules/linmath.c/linmath.h"

int main() { /* ... */ }
```

And then compile with `clang` or `gcc` as usual.

```bash
$ clang main.c  # or, use gcc
$ gcc   main.c
```

You may also use a simpler approach:

```c
// main.c
#include <linmath.h>

int main() { /* ... */ }
```

If you add the path `node_modules/linmath.c` to your compiler's include paths.

```bash
$ clang -I./node_modules/linmath.c main.c  # or, use gcc
$ gcc   -I./node_modules/linmath.c main.c
```

<br>
<br>


[![SRC](https://img.shields.io/badge/src-repo-green?logo=Org)](https://github.com/datenwolf/linmath.h)
[![ORG](https://img.shields.io/badge/org-nodef-green?logo=Org)](https://nodef.github.io)
![](https://ga-beacon.deno.dev/G-RC63DPBH3P:SH3Eq-NoQ9mwgYeHWxu7cw/github.com/nodef/linmath.c)
