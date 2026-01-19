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
#include <linmath.h>

int main() { /* ... */ }
```

Finally, compile while adding the path `node_modules/linmath.c` to your compiler's include paths.

```bash
$ clang -I./node_modules/linmath.c main.c  # or, use gcc
$ gcc   -I./node_modules/linmath.c main.c
```

You may also use a simpler approach with the [cpoach](https://www.npmjs.com/package/cpoach.sh) tool, which automatically adds the necessary include paths of all the installed dependencies for your project.

```bash
$ cpoach clang main.c  # or, use gcc
$ cpoach gcc   main.c
```

<br>
<br>


[![](https://raw.githubusercontent.com/qb40/designs/gh-pages/0/image/11.png)](https://wolfram77.github.io)<br>
[![SRC](https://img.shields.io/badge/src-repo-green?logo=Org)](https://github.com/datenwolf/linmath.h)
[![ORG](https://img.shields.io/badge/org-nodef-green?logo=Org)](https://nodef.github.io)
![](https://ga-beacon.deno.dev/G-RC63DPBH3P:SH3Eq-NoQ9mwgYeHWxu7cw/github.com/nodef/linmath.c)
