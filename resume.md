---
layout: page
title: Resume
---

**Arseny Morozov**

tg: @brocbyte

**Software Engineer - C++, 3D, geometry, systems programming, CAD**

Solid experience in C, C++ and geometric algorithms.

My passion is to dig deeper into software and fight for high performance and smooth user experience.

--------------------------------------------------- **Skills** --------------------------------------------------- 
- geometric algorithms, CAD
- C/C++, Python, Typescript, Vue.js, Three.js, wasm, Qt
- mesh processing: OpenMesh, VTK, Assimp
- graphic APIs: OpenGL, Vulkan, WebGL
- embedded: C, STM32, sensors
- winapi (DirectSound, CoreAudio), X11
- CMake, Git, SVN, conan, Emscripten, selenium
- Agile, Jira, team communication
- English - C1

------------------------------------------------ **Working Experience**------------------------------------------------ 

**Software Engineer - C++/Python/Typescript. [Ledas](https://ledas.com/) (2022 Jun - Now)**
- Project: [Client-server CAD application for orthodontics](https://ledas.com/en/expertise/3d-medical-software/)
    - Triangle mesh processing algorithms using OSS libraries (OpenMesh, Assimp, VTK, draco, three.js)
    - Computational geometry algorithms:
        - Sped up a mesh-to-mesh distance calculation algorithm using uniform grid for raycasting instead of BVH
        - Created a tool for editing distance between meshes
        - Sped up client-based model construction by reusing BVH-instances between meshes
        - Created a tool for keypoint positioning for later mesh segmentation
    - Used [emscripten](https://emscripten.org/) to build mesh-processing code (C++) into wasm modules to reuse on the client and reduce network communication
- Project: Geometric constraint solver for orthodontics
    - Visualization techniques based on mapping 2D points into 3D
    - Mesh processing algorithms (mesh holes filling, computing normals)

**Intern - Coq/Isabelle-HOL. [A.P. Ershov IIS](https://www.iis.nsk.su/en) (2021 Autumn)**
- Project: Proving Algorithm Correctness of Java programs

------------------------------------- **Education & Training: [NSU](https://english.nsu.ru/), IT department** ------------------------------------- 
**2019-2023 -  Bachelor of Computer Science and System Design (GPA 4.98/5.0)**

Research topics:
- *Mesh processing methods for CAD applications*
- *Fast algorithm for retrieving compressed data partially (without decompressing the whole)*

**2023-2025 - MS degree (Internet of Things)**
- FPGA & STM32 programming

---------------------------------------------------  **Pet Projects** --------------------------------------------------- 
* Windows x86-64 user space debugger (C, C++) [repo](https://github.com/brocbyte/oxidbg)
* Triangle mesh segmentation tool (C++, OpenGL) [repo](https://github.com/brocbyte/brocseg)
* Physically-based snow simulation with Material Point Method (C++, CUDA) [repo](https://github.com/brocbyte/realtime-deformations)
* Unix shell: job-control (fg/bg/jobs), stdout/stderr redirection, piping, signals) [repo](https://github.com/brocbyte/gemsh)
* CUDA implementation of "Real-Time Rigid Body Simulation on GPUs" (C++, CUDA, conan) [repo](https://github.com/brocbyte/cuball)
* A minimal X11 & GLX based application for OpenGL rendering without any libs (C++, X11, OpenGL) [repo](https://github.com/brocbyte/octo)
* A not-dictionary-based compression algorithm "CTW" (Python) [repo](https://github.com/brocbyte/ctw)

