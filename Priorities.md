# UnlockGPU: Developer Priorities Document

This is a living document that captures the key technical priorities, pain points, and expectations from the developer community for AMD’s GPU software stack (ROCm, HIP, drivers, libraries, tooling). It complements the [Unlock the GPU Manifesto](https://unlockgpu.org/manifesto) by grounding its demands in concrete, evolving needs.

> 📌 This document changes over time. PRs and issue reports welcome.

---

## 1. Supported Hardware: Stability and Breadth

**Problem:** ROCm has historically supported a limited set of “blessed” GPUs, mostly data center-class and newer SKUs. Older or consumer-tier cards are dropped prematurely.

**Priorities:**
- Ensure ROCm support covers widely available consumer GPUs (e.g. RX 6000/7000 series).
- Guarantee support lifecycles of *at least 5 years* for compute-enabled GPUs.
- Clearly document supported hardware and planned deprecation timelines.
- Avoid “silent” removals of support in point releases.

**Why this matters:**  
Early-career developers, OSS tinkerers, and indie AI researchers often begin with entry-level or used consumer cards. These users form the base of community knowledge, tooling, and advocacy.

---

## 2. Installation and Setup: Simplicity is Power

**Problem:** Getting ROCm working—especially on Ubuntu or with Docker—remains time-consuming and fragile. Common complaints involve kernel mismatches, broken dependency trees, and unclear error messages.

**Priorities:**
- Provide well-maintained Docker containers for major frameworks (e.g. PyTorch, TensorFlow).
- Support LTS Linux distributions on release day (e.g. Ubuntu 24.04).
- Ensure compatibility with container systems (Docker, Podman, Singularity).
- Deliver working ROCm + PyTorch install in 10 minutes or less on supported cards.

**Why this matters:**  
The first impression is critical. Developers comparing AMD and NVIDIA often point to the 6-min vs 6-hr install delta. Usability is market share.

---

## 3. Windows Support: No Longer Optional

**Problem:** ROCm support for Windows is missing or experimental. Workarounds using ONNX/DirectML often underperform.

**Priorities:**
- Ship official ROCm for Windows (even if subset of features).
- Publish roadmap and milestones for Windows compatibility.
- Support popular ML workloads (e.g. inference via PyTorch) on Windows out of the box.

**Why this matters:**  
Most developers and data scientists use Windows for personal or corporate environments. Lack of support blocks adoption entirely.

---

## 4. Libraries and Compatibility Gaps

**Problem:** Even when base frameworks like PyTorch run, many CUDA-optimized libraries (e.g. FlashAttention, LoRA adapters, JAX kernels) do not work on AMD due to missing ROCm equivalents.

**Priorities:**
- Invest in ROCm-native or compatible versions of high-demand libraries.
- Prioritize MLops/AI workloads: LLMs, vision transformers, diffusion models.
- Improve compatibility with Hugging Face Transformers, Optimum, JAX, Triton, etc.
- Maintain and promote equivalence libraries like AiTer, MIOpen, MIGraphX.

**Why this matters:**  
The AI ecosystem moves fast. If ROCm isn’t compatible with next-month’s breakthrough, developers will fall back to CUDA.

---

## 5. Communication and Trust

**Problem:** Developers feel burned by shifting support, unclear messaging, and broken promises. AMD’s forums and docs often lag the reality of developer pain.

**Priorities:**
- Publish changelogs with impact statements (e.g. "ROCm 6.0 removes support for X GPUs").
- Maintain a developer-facing roadmap and known issues tracker.
- Host quarterly community updates (roadmap livestreams, Q&A, GitHub AMAs).
- Fund bug bounties and pay OSS contributors for ROCm improvements.

**Why this matters:**  
The problem is not just code—it’s credibility. AMD must earn trust one version at a time.

---

## 6. Developer Onramps: Lower the Barriers

**Problem:** Many developers don’t even get to “Hello World” with AMD GPUs due to unclear docs or lack of beginner tutorials.

**Priorities:**
- Ship beginner-friendly “ROCm Starter Kit” (scripts + pre-built models).
- Maintain official examples for:
  - Stable Diffusion (Diffusers)
  - LLaMA/LLaVA (Transformers)
  - PyTorch Lightning workflows
- Highlight community guides and contributors.

**Why this matters:**  
Winning developers starts with smooth onboarding. If they succeed quickly, they’ll stay—and teach others.

---

## 7. Strategic Interoperability

**Problem:** Fragmentation across CUDA, HIP, SYCL, OpenCL, and Vulkan confuses developers and dilutes effort.

**Priorities:**
- Invest in SYCL and oneAPI interop via projects like hipSYCL.
- Contribute to open compiler/runtime projects (LLVM, OpenXLA).
- Make ROCm an excellent backend for standardized, cross-platform ML stacks.

**Why this matters:**  
AMD won’t win by building a siloed world. It will win by being the best option in a connected one.

---

## Tags and Wishlist (for GitHub tracking)

We recommend tagging issues and PRs with:

- `driver-support`
- `installation`
- `pytorch`
- `windows`
- `low-end-gpus`
- `ml-library-gap`
- `docs-and-onboarding`
- `sycl-openxla-interop`

---

*Maintained by the UnlockGPU community. Join the conversation and contribute your pain points, ideas, and improvements.*

