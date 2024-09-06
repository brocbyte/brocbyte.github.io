---
layout: page
title: Resume
---

# Arseny Morozov

**Software Engineer - C++, 3D, geometry, low level programming, CAD**

I am a software engineer with solid experience in C, C++ and geometric algorithms.

My passion is to dig deeper into software and fight for high performance and smooth user experience.

---

## Skills
- geometric algorithms, CAD
- C/C++, Python, Typescript, Vue.js, Three.js, wasm
- mesh processing: OpenMesh, VTK, Assimp
- graphic APIs: OpenGL, Vulkan, WebGL
- winapi (DirectSound, CoreAudio), X11
- CMake, Git, SVN, conan, Emscripten, selenium
- Agile, Jira, team communication
- English - C1

## Working Experience

### Software Engineer. [Ledas](https://ledas.com/) (2022 Jun - Now)

- #### Project: [Client-server CAD application for orthodontics (C++/Typescript)](https://ledas.com/en/expertise/3d-medical-software/)
    - Used third-party libraries for basic operations on 3D meshes (OpenMesh, Assimp, VTK, draco, three.js)
    - Implemented several computational geometry algorithms:
        - Sped up a mesh-to-mesh distance calculation algorithm using uniform grid for raycasting instead of Bounding Volume Hierarchy
        - Created a tool for editing distance between meshes
        - Sped up client-based model construction by reusing BVH-instances between meshes
        - Created a tool for keypoint positioning for later mesh segmentation
    - Used [emscripten](https://emscripten.org/) to build mesh-processing code (C++) into wasm modules to reuse on the client and reduce network communication

- #### Project: Geometric constraint solver application for orthodontics
    - Implemented a visualization technique based on mapping 2D points into 3D
    - Implemented some mesh processing algorithms (mesh holes filling, computing normals)

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

## Pet Projects

Windows x86-64 user space debugger, (C, C++) [repo](https://github.com/hardworkar/oxidbg)

Vulkan-driven renderer (C, Vulkan) [repo](https://github.com/hardworkar/oxigine)

Physically-based snow simulation with Material Point Method (C++, CUDA) [repo](https://github.com/hardworkar/realtime-deformations)

CUDA implementation of "Real-Time Rigid Body Simulation on GPUs" (C++, CUDA, conan) [repo](https://github.com/hardworkar/cuball )

Unix shell: job-control (fg/bg/jobs), stdout/stderr redirection, piping, signal handling) [repo](https://github.com/hardworkar/gemsh)

A minimal X11 & GLX based application for OpenGL rendering without any libs (e.g. ~~GLFW~~, ~~GLAD~~) (C++, X11, OpenGL) [repo](https://github.com/hardworkar/octo)

Implemented a not-dictionary-based compression algorithm "CTW" (Python) [repo](https://github.com/hardworkar/ctw)

