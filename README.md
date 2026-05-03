# Hi, I'm Sumedha Umesh Kulkarni 👋

**Software Engineer** working across the stack that sits between **metal and models**: production **automotive C++** (HAL, Bluetooth, bring-up), **LLM systems** (RAG, agents, on-device inference), and **robotics / AAOS-style** platforms — plus **MERN** and **GCP** when the product needs a web or cloud spine.

Los Angeles, California · Open to roles · **F1-OPT + STEM** · Open to relocation

---

## 👤 About me

I build software when **timing, hardware, and messy real-world data** all push back at once — battery paths through a HAL, Bluetooth stacks that need **GDB** and **DLT-Viewer**, PDFs and scans that won’t parse cleanly, or an ADAS pipeline that has to run in **Docker** with **Fast DDS** tuned for latency.

**Track record:** At **Mercedes-Benz** I owned pieces of the **C++17** path between HAL and apps (**BlueGo**, **DeviceManager RPC**), chased **Bluetooth** / DeviceManager defects with core dumps, raised **GTest** coverage **~30%**, and ran **hardware bring-up and flashing** across **45+ tasks** (ET-framework, Monaco). At **Deep Cognition** I shipped a **Haystack** RAG stack (**SentenceTransformers**, **Anthropic Claude**) wired into **LibreChat** for **500+ documentation repos**, and an ingestion path (**Playwright** EML→PDF, **OCR**, **200+ docs/day**) that cut invoice turnaround **~65%**.

**Academic & personal work** spans **Zephyr / Cortex-M** firmware with **QEMU CI**, **ROS 2 Humble** perception and fusion toward **FCW/LDW**, **Android Automotive** modules with **AIDL** and **Room**, **LangGraph** multi-agent research, **FastAPI + llama.cpp** on-device voice agents, and a **gRPC** file-sync core with a roadmap toward **Merkle trees, inotify, and conflict policies**.

**Now:** MS in **Computer Science** at **USC** (Los Angeles). Authorized to work in the US on **F1-OPT with STEM extension**; open to relocation. I like problems that mix **hardware, backend, and ML** — and I write docs teammates can actually use.

---

## 🚀 What I'm working on

Closing out my **MS CS at USC** while pushing **ROS 2** work (**perception**, sensor replay, fusion-style tracking) and **ML-adjacent features** where constraints matter: **grammar-bound LLM outputs**, **tool routing under latency budgets**, and **RAG / agent** flows that stay observable and cite sources — not just “call an API and hope.”

---

## 🛠️ Tools & technologies

| Area | Examples |
|------|----------|
| 💻 **Languages** | C++17, Python, Kotlin, JavaScript / TypeScript |
| 🔧 **Embedded & vehicle ECU-style** | Zephyr RTOS, Cortex-M, QEMU, GDB, DLT-Viewer; BlueGo / DeviceManager RPC, ET-framework, Monaco bring-up |
| 🚗 **Robotics & infotainment** | ROS 2 Humble, Docker, Eigen, OpenCV, Foxglove, Fast DDS; Android Automotive, AIDL, Room, Gradle |
| 🌐 **Services & sync** | FastAPI, Flask, REST, WebSockets, gRPC, Protobuf, CMake; MERN-style stacks; GCP |
| 🤖 **AI / ML** | LangGraph, Haystack, SentenceTransformers, Anthropic Claude, Whisper, llama.cpp, Tavily, Playwright, OCR / doc pipelines |
| 🤝 **Quality & delivery** | GoogleTest, GitHub Actions / Ubuntu CI, Markdown / architecture docs |

---

## 💼 Experience

### Deep Cognition — AI Intern · Remote  
*June 2025 – August 2025*

- Built a **Haystack-based RAG** pipeline (Markdown split/index, SentenceTransformers, **Anthropic Claude**) — **~37% lower retrieval latency**.
- **Real-time Q&A** over **500+ documentation repos** in LibreChat via **Flask** REST JSON endpoints.
- **~65% faster invoice ingestion**: EML→PDF with **Playwright**, **OCR** metadata from PDFs/images, **200+ documents/day** into an AI document pipeline.

### Mercedes-Benz — Software Developer · India  
*August 2023 – May 2024*

- **C++17** HAL↔app path with **BlueGo** and **DeviceManager RPC** for battery data, persistence, and real-time UI alerts.
- **Bluetooth** and DeviceManager debugging with **GDB** and **DLT-Viewer**; core dumps; **~20% reduction** in related bug incidence.
- **+30% code coverage** with **GTest** automation.
- **Hardware bring-up / flashing** for **45+ tasks** (ET-framework, Monaco).

### Mercedes-Benz — Intern · India  
*February 2023 – July 2023*

- **Python CLI** on Linux for automated HW/SW testing — adopted by **10+ engineers**.

---

## Projects

Full write-ups, visuals, and architecture notes: **[portfolio](https://sumedhak.netlify.app)**.

**Deep Research Agent**

**Stack:** LangGraph, Python, Tavily, Anthropic Claude  

A **LangGraph** multi-agent system that **decomposes open-ended questions**, runs **parallel research** across many web sources, and returns **structured, citation-backed reports** — not a single monolithic prompt. **Planner, search, and synthesis** agents share state; **Tavily** and **Claude** sit behind **extensible tools** and explicit **citation policies** so answers stay traceable.

- Parallel research across **500+ sources**; outputs include citations; **~60% faster** end-to-end research turnaround vs the prior manual flow.
- Clear separation between **planning, retrieval, and synthesis**; room to plug in new tools and tighten what counts as a valid citation.

---

**Concierge**

**Stack:** Python, FastAPI, llama.cpp, WebSockets, Whisper  

An **in-car, on-device** stack around a **~1.2B** local LLM: a **two-stage gate + generator** with **GBNF**-constrained **JSON** so the model can’t improvise invalid tool calls. **Whisper** does speech; **llama.cpp** runs the model; **FastAPI** and **WebSockets** keep the loop under a **~3s** “tick” with **typed intents**, **per-call timeouts**, and **intent decomposition** for compound voice commands (e.g. routes and weather) hitting **Overpass**, **Open-Meteo**, **OSRM**, and **Nominatim**.

- **GBNF** keeps tool calls valid; LLM work budgeted to **~10%** of the **3s** tick so most time goes to real I/O and routing.
- **Sub-second** routing to external APIs; designed for **low-latency** in-vehicle use, not a chatty server round-trip for every nuance.

---

**Embedded Health-Monitor Firmware**

**Stack:** Zephyr RTOS, C++17, Cortex-M, QEMU, GoogleTest  

**C++17** on **Zephyr** for **Cortex-M**: **drivers, services, and algorithms** in a **3-tier** layout, with **QEMU** in **CI** so logic is tested on every push. **Host-side GoogleTest** covers signal processing and state without flashing hardware. **HR** uses an **IIR bandpass**, peak detect → **BPM**; **activity** uses **IMU variance** — **coefficients and thresholds** are **tunable** for different boards and noise floors.

- **QEMU** regression in CI; same code paths stressed as on device.
- Signal chain and activity logic verified with **GoogleTest** before bring-up, reducing “flash and pray” debug cycles.

---

**MOSAIC**

**Stack:** ROS 2 Humble, Docker, Python, C++17, Eigen, OpenCV, Foxglove  

A **Dockerized** **Ubuntu 22.04** **ROS 2** stack: **bag replay**, **camera + LiDAR** perception, **association + EKF**-style **fusion tracking**, and **ADAS-style** outputs (**FCW**, **lane-departure**-like warnings). **Custom `mosaic_msgs`**, **Python** and **C++** nodes, **YAML/launch** wiring, and **Fast DDS** settings tuned for **container** networking. **Foxglove** is optional for visualization. Architecture is built so **models and sensor loaders** can be **swapped** without rewiring the whole graph.

- **KITTI**-style replay; end-to-end path from sensors through fusion to **FCW / LDW**-style warnings.
- **Kit** for experiments: same launch story in dev and CI-style environments.

---

**CarOSMini**

**Stack:** Kotlin, Android Automotive, AIDL, Room, Gradle  

A **multi-module** **Android Automotive**-style build: **core AIDL services** (e.g. **IProfileService**, **IPhoneConnectionService**), a **launcher**, and **stub feature apps** — with a **documented dual-emulator** workflow (AAOS + phone) for realistic testing. **Bluetooth ACL** events (**ACTION_ACL_CONNECTED**) map a **MAC** to **Room**-backed **device → profile** links, then **broadcast** profile changes to the shell. **Gradle** is split so **core-service**, **launcher**, and **features** stay isolated.

- **Room** schema for **device_profile_links**; **ProfileService** owns the truth for “which phone maps to which profile.”
- Reproducible **AAOS + phone** bring-up so Bluetooth flows are testable without a full car bench.

---

**Distributed File Sync Engine**

**Stack:** C++17, gRPC, CMake, Protobuf  

**Phase 1** of a **bidirectional directory sync** system: **`sync_client` / `sync_server`** over **gRPC**, **structured logs**, **metrics CSVs**, and **clean shutdown** — a foundation before **Merkle / rolling-hash diffs**, **inotify**-driven sync, and **conflict policies**. **CMake** + **Protobuf** define the RPC surface; **paired log + metrics directories** support post-run analysis.

- **CI on Ubuntu 24.04**; RPC boundary locked in early so sync semantics can evolve behind a stable API.
- Roadmap is explicit: **Merkle trees**, **delta sync**, **inotify**, and **conflict resolution** — this repo is the **bootstrap**, not the finished product.

---

## 📬 How to reach me

| Channel | Detail |
|--------|--------|
| ✉️ **Email** | [sumedhau@usc.edu](mailto:sumedhau@usc.edu) |
| 💼 **LinkedIn** | [linkedin.com/in/SumedhaUmeshKulkarni](https://www.linkedin.com/in/SumedhaUmeshKulkarni/) |
| 🌐 **Portfolio** | [sumedhak.netlify.app](https://sumedhak.netlify.app) |

---

Thanks for visiting 🙏
