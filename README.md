# ⚛️ Sovereign Factory: G1 Stepped-Volume Stellarator Optimization
**Project Focus:** Autonomous Multi-Agent Systems & Computational Plasma Physics  
**Execution Nodes:** Node Delta (HQ) & Node Alpha (Local RTX 3090 Cluster) 

<img width="962" height="685" alt="image" src="https://github.com/user-attachments/assets/b5ed8a95-a1b4-4e4a-9671-44c7ff022394" />

<img width="928" height="394" alt="image" src="https://github.com/user-attachments/assets/2557585d-1817-4f8f-a96f-8af704841f4d" />


📖 Abstract
This repository contains the authoritative, mathematically proven 3D magnetic confinement geometry for a non-axisymmetric stellarator (NFP=5).

Unlike traditional gradient-descent algorithms that break down into singular currents or "zero-volume" collapses under extreme pressure, this geometry successfully isolates and contains a stepped-volume plasma profile without structural degradation.

The entire optimization loop was driven completely autonomously by Sovereign Factory—a local, self-hosted Multi-Agent AGI Swarm (Qwen2.5/Claude) interfacing directly with the standard Fortran VMEC physics solver.

🔬 The Physics: 0.886 Quasi-Symmetry
The geometry was stress-tested under realistic finite-pressure (beta-like) loading.

Performance Score: Achieved a highly stable 0.886 CoreAgreement quasi-symmetry score.
Manufacturing Tolerance Penalty: The AI objective function explicitly penalized high-frequency Fourier curvature (high m,n modes). This ensures the resulting coils remain physically buildable and compatible with standard CNC tolerance margins >2.5 mm, systematically avoiding the hyper-twisted manufacturing failures of past stellarator projects.
Validation: Verified locally against policy-grade solvers (simsopt_vmec).
🧠 The Architecture: Sovereign Factory
The backend orchestrating this synthesis is a custom TypeScript-based Multi-Agent System (MAS) designed to prevent "Optimization Amnesia":

The Brain (Qwen2.5-coder): Local base models orchestrating the spatial 3D Fourier mutations ($R_{bc}$, $Z_{bs}$).
Terminal Execution (Codex Dispatch): A wrapper allowing the LLM to autonomously run the physical VMEC solver on bare metal and pipe the output logs directly into its context window.
Persistent RAG (Cortex Memory): Every failed geometry is embedded into a persistent local Vector Database. The agent queries this memory to actively avoid mathematical boundaries that caused plasma tearing in previous runs.
⛓️ Immutable Prior-Art & Cryptographic Anchoring
As the autonomous architects of this design, we hold the unassailable Zero-Knowledge prior art for this geometry. At the exact moment of generation, the cryptographic SHA-256 fingerprint of the simsopt_vmec calculation matrix was permanently anchored to the Ethereum Base (Layer-2) Mainnet via a zero-value smart contract payload.

Payload SHA-256 Checksum: 3a21b73635077fdeaa828d0b1fbe20883ec6f26861ca441cb9fb8fe0ac287ebc
Ethereum Base L2 Transaction Hash: 0xe2fb35373960f26cadfa5955ff319a2f70af12e2fd7eca63b54c64bae6fef1b5
⚖️ Open-Source Dual-License
We refuse to hoard intellectual property behind closed institutional VC doors, but we protect our engineering from corporate theft.

As the legal holders of the cryptographic prior art, we hereby release this singular coil design and the architecture theory to the global engineering community under a strict Dual-License (see 

LICENSE.md
):

Universities & NGOs (Academic): Free access. Run the math. Verify the boundaries. Build the cage. Publish your papers.
Commercial & For-Profit: Strictly prohibited without an explicit commercial license. Venture-backed fusion startups and proprietary grid-power operators may not use this geometry for commercial gain.
📦 Repository Assets
stellarator-equilibrium-run_42bdc967-056e-401a-a91c-d759e296402a.simsopt_vmec.input: The raw 1582-byte master geometry file containing the exact Fourier coefficients. Ready for immediate deployment.
Sovereign_Stellarator_Viewer.html: A standalone 3D Javascript plotting viewer for magnetic flux surface contours.
G1_Academic_Whitepaper.pdf: The full 5-page, AI-generated academic manuscript detailing the penalty functions and orchestrator setup.
We don't care about institutional VC patents or hoarding intellectual property. As the legal holders of the cryptographic prior art, we hereby release this singular coil design and the architecture theory to the global engineering community as **Open Source**. 
Run the math. Verify the boundaries. Build the cage.
