## Why curated AWESOME lists and RSS feeds matter so much

*We'd never keep up without curated reading lists that help us build RSS feeds ... especially in rapidly evolving industries with lots of investment driving R&D and new theoretical work.*

A rapidly developing research and development space such as eGPUs/eTPUs connectivity illustrates why. But, more generally, it is important to curate repositories of lists of AWESOME blogs and online publications by independent thinkerers, industry experts and research institutions ... by following these curated lists, or the abstracts from linked RSS feeds, one is better able to an eye on key things.  

So it's not JUST researchers/labs involved that developing as well as the conferences and workshops focused on HPC, cloud computing, and server technologies, as these often serve as a place for new ideas in cutting-edge research and development in eGPU/eTPU connectivity to emerge ... we ALSO continue to learn from [Archetypal Repository](https://github.com/sindresorhus/awesome) which laid the foundation for the broader archetypal example of listification in [the Awesome Lists of Awesome Lists](TheArchetype.md).

## Awesome Hardware Relevant To eGPUs 

While [Oculink 2](https://www.howtogeek.com/what-is-oculink/) is well known to followers of things like the [eGPU forum](https://egpu.io/) and has established itself as the current champion for connecting external GPUs (eGPUs) to rackmount servers, the future holds some exciting possibilities for even faster and more efficient connections. 

Here are a few potential contenders for the "next big thing" in eGPU technology:

* PCI Express (PCIe) 6.0 and 7.0: The [PCI-SIG](https://pcisig.com/) is responsible for developing and enhancining the PCIe standard, crucial for ensuring compatibility and interoperability of eGPU/eTPU solutions. The next major revision, 7.0 of PCIe is already on the horizon and the not-quite-available BUT close-to-being-delivered standard PCIe 6.0 will deliver significant bandwidth improvements over PCIe 5.0, currently employed by Oculink 2. Optimizations of PCIe 6.0 could actually double the theoretical bandwidth yet again, potentially exceeding the expected 128 GB/s per lane. While motherboards and eGPUs supporting PCIe 6.0 will take some time to become fully mainstream, it represents a clear evolutionary step for high-performance computing requiring massive GPU acceleration.

* NVLink and other proprietary, eg AMD, Intel, Broadcom, etal, high-speed interconnects: Manufacturers like NVIDIA [and tons of would-be NVIDIA competitors and startups hoping to be acquired] are hyper-motivated by the massive investor interest in developing their own interconnects like NVLink, offering even higher bandwidth and lower latency compared to PCIe. While currently limited to specific systems and GPUs, advancements in these proprietary technologies could challenge the dominance of PCIe in the future. The potential downside of proprietary solutions is their limited compatibility and potential vendor lock-in, requiring careful consideration by users.

* [CXL (Compute Express Link)](https://www.computeexpresslink.org/): Compute Express Link™ (CXL™) is an industry-supported [standard specification, currently at rev 3.1](https://www.computeexpresslink.org/_files/ugd/0c1418_129f28a1687445098e8851a3a8b3a5ea.pdf) cache-coherent interconnect for processors, memory expansion and accelerators which focuses on providing a high-bandwidth, low-latency link between CPUs and accelerators like GPUs. While not directly replacing eGPU connections, CXL could enable tighter integration and efficient data sharing between the CPU and GPU, unlocking additional performance gains. CXL is still in its early stages of adoption, but its potential for optimizing data movement and communication within the server could significantly impact future eGPU implementations.

* [Wireless 6G Technologies such Terahertz (THz)](https://www.connectedpapers.com/main/423352ee662bca36db73db0f59f6b9cada4fafc1/Seven-Defining-Features-of-Terahertz-(THz)-Wireless-Systems%3A-A-Fellowship-of-Communication-and-Sensing/graph): Of course, this might SEEM like it's unduly futuristic, advancements in wireless communication technologies like [Terahertz (THz)](https://arxiv.org/abs/2102.07668) and other [advances in multiplexing and other things the application of information theory](https://arxiv.org/list/cs.IT/23) could eventually pave the way for truly cable-free eGPU connections. *JUST IMAGINE* the flexibility and efficiency of eliminating bulky cables without compromising performance. These option remains far from practical implementation, but the potential long-term benefits for not just simply for data center design and maintenance on Earth, but Universal computing by satellites and exploratory vehicles in deep space are undeniable.

* [Hardware Architecture in general](https://arxiv.org/list/cs.AR/23): It's not just about GPUS, TPUs, accelerators, and other hardware components ... it's tough to predict the economic importance of a specific different developments in hardware architecture or the manufacturing technologies necessary to realize those architectures ... but there are plenty of research institutions that not only do theoretical research in hardware, but are also particularly motivated by practical use cases for GPU/TPU clusters in their other fields of research ... of course, this includes those such as Lawrence Livermore National Laboratory and Max Planck Institute for Computer Science, but practically it's basically every research institution in the world with something like a computer engineering departrment on campus ... moreover, there are plenty of on-going academic research projects from a variety of different quarters publishing pre-print papers in this space ... so [hardware architecture](https://arxiv.org/list/cs.AR/23) is just about things like quantum computing or RISC-V open source processor architecture but also plenty of other different new theoretical-yet-close-to-practical developments in parallel computing.

## Open Source Communities in eGPU Realm

There are ALSO several relevant Open Hardware/Open Software Communities such as:

* [Open Compute Project](https://www.opencompute.org/): Open-source community focused on developing efficient server and data center designs, with potential applications for eGPU/eTPU connectivity.

* [OpenPOWER Foundation](https://openpowerfoundation.org/): Open-source community focused on developing high-performance computing solutions, with potential applications for eGPU/eTPU connectivity.

* [OpenACC](https://www.openacc.org/): Open-source community focused on developing high-performance computing solutions, with potential applications for eGPU/eTPU connectivity.

* [OpenMP](https://www.openmp.org/): Open-source community focused on developing OpenMP API specification for parallel programming as well as other high-performance computing solutions, with potential applications for eGPU/eTPU connectivity.

* [OpenCL](https://www.khronos.org/opencl/): Open-source community focused on developing high-performance computing solutions, with potential applications for eGPU/eTPU connectivity.

* [OVS (Open Virtual Switch)](https://www.openvswitch.org/): Open-source project for production quality, multilayer open virtual switch which would provide high-performance virtual networking solutions, potentially enabling efficient data transfer for virtualized GPUs/TPUs.

* [DPDK (Data Plane Development Kit)](https://www.dpdk.org/): Open-source framework for high-performance networking applications, with potential applications in optimizing network traffic for eGPUs/eTPUs.

## eGPU-in-Software and GPU/TPU Virtualization

The rise of GPU/TPU virtualization and cloud-based access to GPUs could transform the eGPU landscape. Instead of physical connections, users might access remote GPUs through virtualized pools, simplifying management and scaling based on demand. This shift would require robust virtualization technologies and efficient network infrastructures, but could dramatically change how businesses approach and utilize GPUs for various workloads.

[Linux Kernel GPU Virtualization](https://www.kernel.org/doc/html/latest/gpu/): The Linux kernel [Direct Rendering Manager (DRM)](https://en.wikipedia.org/wiki/Direct_Rendering_Manager) layer contains code intended to support the needs of complex graphics devices, usually containing programmable pipelines well suited to 3D graphics acceleration. Graphics drivers in the kernel may make use of DRM functions to make tasks like memory management, interrupt handling and [Direct Memory Access (DMA)](https://en.wikipedia.org/wiki/Direct_memory_access) easier, and provide a uniform interface to applications. The DRM layer contains code intended to support the needs of complex graphics devices, usually containing programmable pipelines well suited to 3D graphics acceleration. Graphics drivers in the kernel may make use of DRM functions to make tasks like memory management, interrupt handling and DMA easier, and provide a uniform interface to applications.

