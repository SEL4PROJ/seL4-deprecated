<!--
  Copyright 2019, Data61
  Commonwealth Scientific and Industrial Research Organisation (CSIRO)
  ABN 41 687 119 230.

  This software may be distributed and modified according to the terms of
  the BSD 2-Clause license. Note that NO WARRANTY is provided.
  See "LICENSE_BSD2.txt" for details.

  @TAG(DATA61_BSD)
-->
# seL4-deprecated

Provides a location to place projects that are no longer maintained and have
been deleted from their previous repositories.

See [seL4-deprecated-manifests](https://github.com/SEL4PROJ/seL4-deprecated-manifests) for pinned versions of projects that once worked
together.

Use at your own discretion.


## Contents

- libsel4arm-vmm: An Arm-only hardware virtualisation library.
  Previously located in seL4_project_libs.  Became libsel4vm and libsel4vmmplatsupport.
- libsel4vmm: A x86-only hardware virtualisation library.
  Previously located in seL4_libs. Became libsel4vm and libsel4vmmplatsupport.
- libsel4pci: A PCI emulation driver for vmms. Previously located in seL4_project_libs.
  Was merged into libsel4vmmplatsupport.
- libsel4vmmcore: Virtualisation utilities for vmms. Previously located in seL4_project_libs.
  Was merged into libsel4vmmplatsupport.
- patches/0001-Use-deprecated-libraries.patch: Patch for https://github.com/seL4/camkes-vm to use these deprecated libraries.
- patches/0001-Use-deprecated-library-paths.patch: Patch for https://github.com/SEL4PROJ/camkes-arm-vm to use these deprecated libraries.
- FindseL4-deprecated.cmake: CMake package file for importing these libraries into a CMake project.
