---
layout: page
title: Resume
---

# Arseny Morozov

**Software Engineer - C++, 3D, geometry, low level programming, CAD**

I am a software engineer with solid experience in C, C++ and geometric algorithms.
My passion is to dig deeper into software and fight for high performance and smooth user experience.

---

## Working Experience

### Software Engineer. [Ledas](https://ledas.com/) (2022 Jun - Now)

- #### Project: [Client-server CAD application for orthodontics](https://ledas.com/en/expertise/3d-medical-software/)

    - Sped up a mesh-to-mesh distance calculation algorithm using uniform grid for raycasting instead of Bounding Volume Hierarchy (Typescript, C++)
    - Mesh processing (fill mesh holes, flip normals) (C++, VTK)
    - Automatic tool for editing distance between meshes (Typescript, three.js)
    - Used [emscripten](https://emscripten.org/) to build server-side mesh-processing code (C++) into wasm modules to reuse code on the client and reduce network communication
    - Fixed bugs & implemented features using open-source external libraries (OpenMesh, Assimp)
    - Mesh loading stage was sped up using [draco](https://google.github.io/draco/) library for mesh compression. It was included in an existent Websocket-based message communication. (Typescript, C++, CMake)
    - Client-based model construction was sped up by reusing BVH-instances between meshes (Typescript, three.js)
---
- #### Project: Geometric constraint solver application for orthodontics
    - Implemented a visualization technique translating 2D points into 3D

### Intern. [A.P. Ershov IIS](https://www.iis.nsk.su/en) (2021 Autumn)

- #### Project: Proving Algorithm Correctness of Java programs
    - Proved properties of Java-based class implementations (Coq, Isabelle/HOL)

## Education & Training: [NSU](https://english.nsu.ru/), IT department

### 2019-2023 -  Bachelor of Computer Science and System Design (GPA 4.98/5.0)

Research topics:

- *Mesh processing methods for CAD applications*
- *Fast algorithm for retrieving compressed data partially (without decompressing the whole)*

### 2023-2025 - MS degree (Internet of Things)

- FPGA & STM32 programming

## Skills
- Geometric Algorithms, CAD
- C/C++, Python, Typescript, Vue.js, Three.js, wasm
- OpenMesh/VTK/Assimp, OpenGL, X11, Emscripten, DirectSound, CoreAudio, Vulkan
- CMake, Git, SVN, conan
- Agile, team communication
- English - C1

## Pet Projects

Windows x86-64 user space debugger, (C, C++) [repo](https://github.com/hardworkar/oxidbg)

Vulkan-driven renderer (C, Vulkan) [repo](https://github.com/hardworkar/oxigine)

Material Point Method for physically-based snow simulation (C++, CUDA) [repo](https://github.com/hardworkar/realtime-deformations)

CUDA implementation of "Real-Time Rigid Body Simulation on GPUs" (C++, CUDA, conan) [repo](https://github.com/hardworkar/cuball )

Little unix shell: job-control (fg/bg/jobs), stdout/stderr redirection, piping, signal handling) [repo](https://github.com/hardworkar/gemsh)

A minimal X11 & GLX based application for OpenGL rendering without any libs (e.g. ~~GLFW~~, ~~GLAD~~) (C++, X11, OpenGL) [repo](https://github.com/hardworkar/octo)

Implemented a not-dictionary-based compression algorithm "CTW" (Python) [repo](https://github.com/hardworkar/ctw)

