A C++ graphics library inspired by [Processing](https://processing.org). In development. 

## features - development status
- [x] orthographic and perspective projection
- [x] window handling
- [x] complete matrix handling
- [x] 2D textures
- [x] instancing
- [ ] text rendering
- [ ] light
- [ ] face culling

## usage

```c++
#include "fly/fly.h"

int main(){

  fly::createWindow("parallelogram", 800, 600);
  fly::initialize(fly::projectionMethod::ORTHO);

  for(; fly::running(); fly::update()){ //render loop

    //...
  }

  fly::terminate();
  return 0;
}
```

Check [examples](https://github.com/flightcoded/fly-graphics/tree/master/examples) also.

## dependencies
* [GLAD](https://glad.dav1d.de) (configured for OpenGL 3.3 Core)
* [GLFW](https://www.glfw.org)
* [GLM](https://github.com/g-truc/glm)
* [stb_image](https://github.com/nothings/stb/blob/master/stb_image.h)

There is a complete Visual Studio project with all dependencies linked and included under [releases](https://github.com/flightcoded/fly-graphics/releases).
