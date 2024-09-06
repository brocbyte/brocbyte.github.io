---
layout: page
title: Resume
---

# Arseny Morozov CV

Software Engineer - 3D, geometry, performance, CAD

arsmoroz@ya.ru

tg: @brocbyte

[https://github.com/brocbyte](https://github.com/brocbyte/)

---

## Working Experience

### Software Engineer. [Ledas](https://ledas.com/). Novosibirsk, Russia. (2022 Jun - Now)

***Project:** [Client-server CAD application for orthodontics](https://ledas.com/en/expertise/3d-medical-software/)*

- Sped up a mesh-to-mesh distance calculation algorithm from 3s to 0.02s using uniform grid for raycasting instead of Bounding Volume Hierarchy (Typescript, C++)
- Mesh processing (fill mesh holes, flip normals) (C++, VTK)
- Automatic tool for editing distance between meshes (Typescript, three.js)
- Used [emscripten](https://emscripten.org/) to build server-side mesh-processing code (C++) into wasm modules to reuse code on the client and reduce network communication
- Fixed bugs & implemented features using open-source external libraries (OpenMesh, Assimp)
- Mesh loading stage was sped up using [draco](https://google.github.io/draco/) library for mesh compression. It was included in an existent Websocket-based message communication. (Typescript, C++, CMake)
- Client-based model construction was sped up by reusing BVH-instances between meshes (Typescript, three.js)

### Intern. [A.P. Ershov IIS, Siberian Branch of the Russian Academy of Sciences](https://www.iis.nsk.su/en). Novosibirsk, Russia. (2021 Autumn)

- ***Project:*** Proving Algorithm Correctness of Java programs
    - Proved properties of Java-based class implementations (Coq, Isabelle/HOL)

## Education & Training

### 2019-2023 -  Bachelor of Computer Science and System Design (GPA 4.98/5.0)

[Novosibirsk State University](https://english.nsu.ru/). Information Technology department.

Research topics:

- *Mesh processing methods for CAD applications*
- *Fast algorithm for retrieving compressed data partially (without decompressing the whole)*

### 2023-2025 - Master’s degree (Internet of Things)

[Novosibirsk State University](https://english.nsu.ru/). Information Technology department.

- FPGA & STM32 programming

## Skills

- C/C++, Python, Typescript/JavaScript, Vue.js, Three.js
- OpenMesh/VTK/Assimp, OpenGL, X11, Emscripten, DirectSound, CoreAudio, Vulkan
- CMake, Git, SVN, conan
- Agile, team communication
- English - C1

## Pet Projects

### https://github.com/hardworkar/oxidbg

- Windows debugger

### https://github.com/hardworkar/oxigine (C, Vulkan)

- Vulkan-driven renderer

### https://github.com/hardworkar/cuball (C++, CUDA, conan)

- CUDA-based implementation of "Real-Time Rigid Body Simulation on GPUs" [from GPU Gems 3] paper

### https://github.com/hardworkar/realtime-deformations (C++, CUDA)

- Material Point Method for physically-based snow simulation, used several papers as a reference.

### https://github.com/hardworkar/gemsh (C, Unix)

- a shell: job-control (fg/bg/jobs), stdout/stderr redirection, piping, signal handling.

### https://github.com/hardworkar/octo (C++, X11, OpenGL)

- A minimal X11 & GLX based application for OpenGL rendering without using any additional libs (e.g. ~~GLFW~~, ~~GLAD~~)

### https://github.com/hardworkar/ctw (Python)

- Implemented [a fun not-dictionary-based compression algorithm](https://en.wikipedia.org/wiki/Context_tree_weighting).
