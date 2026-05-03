# Hi, I'm Sumedha Umesh Kulkarni 👋

**Software Engineer** — Embedded Systems, Full-Stack (MERN), and AI/ML (RAG, OCR, NLP).

Los Angeles, California · Open to roles · **F1-OPT + STEM** · Open to relocation

---

## 👤 About me

I'm a Software Engineer with experience in **Embedded Systems** (C++, Bluetooth, RTOS), **Full-Stack Development** (MERN, REST APIs, GCP), and **AI/ML** (RAG pipelines, OCR, NLP). I'm authorized to work in the US on **F1-OPT with STEM extension** and open to relocation.

I gravitate toward problems where software has to behave when the real world isn't cooperating.

**Background in brief:** MS in Computer Science at **USC** (Los Angeles). I've shipped **automotive firmware** at Mercedes-Benz (Bluetooth, HAL, bring-up) and **AI tooling** at Deep Cognition (RAG, documentation, messy PDFs). I like work that mixes **hardware, backend, and ML** — with room for dry humor.

---

## 🚀 What I'm working on

Finishing my degree at USC while digging deeper into **ROS 2 and perception**, and shipping **ML-adjacent features** responsibly in personal and academic projects.

---

## 🛠️ Tools & technologies

| Area | Examples |
|------|----------|
| 💻 **Languages** | C++17, Python, Kotlin, JavaScript/TypeScript |
| 🔧 **Embedded & systems** | Zephyr RTOS, Cortex-M, QEMU, GDB, BlueGo / DeviceManager RPC, ET-framework |
| 🚗 **Robotics & automotive** | ROS 2 Humble, Docker, Eigen, OpenCV, Foxglove; Android Automotive, AIDL, Gradle |
| 🌐 **Full-stack & APIs** | FastAPI, Flask, REST, WebSockets, gRPC, Protobuf, CMake, MERN ecosystem, GCP |
| 🤖 **AI / ML** | LangGraph, Haystack, SentenceTransformers, Anthropic Claude, Whisper, llama.cpp, Tavily, OCR pipelines |
| 🤝 **Quality & delivery** | GoogleTest, CI (GitHub Actions / Ubuntu), Markdown docs |

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

Full stories, visuals, and architecture notes live on my **[portfolio](https://sumedhak.netlify.app)**.

**Deep Research Agent**

**Stack:** LangGraph, Python, Tavily, Anthropic Claude  

LangGraph multi-agent system with parallel research and citation-backed reports.

- Parallel research across **500+ sources**; citation-backed outputs; **~60% faster** research turnaround vs prior workflow.
- Planner / search / synthesis agents with shared state; Tavily + Claude; extensible tools and citation policies.

**Concierge**

**Stack:** Python, FastAPI, llama.cpp, WebSockets, Whisper  

On-device in-car AI agent with grammar-constrained LLM output and sub-second tool routing.

- **GBNF** grammar-constrained JSON; LLM calls capped to **~10%** of a **3s** tick.
- Intent router → **Overpass**, **Open-Meteo**, **OSRM**, **Nominatim** under **1s**.

**Embedded Health-Monitor Firmware**

**Stack:** Zephyr RTOS, C++17, Cortex-M, QEMU, GoogleTest  

Zephyr on Cortex-M with layered architecture and host-side GoogleTest.

- **3-tier** architecture; **QEMU CI**; HR pipeline (IIR bandpass, peak detect → BPM) + activity (IMU variance) tested with **GoogleTest** without flashing.

**MOSAIC**

**Stack:** ROS 2 Humble, Docker, Python, C++17, Eigen, OpenCV, Foxglove  

ROS 2 ADAS scaffold: camera + LiDAR perception, fusion tracking, FCW/LDW.

- Custom msgs, **KITTI** replay, Python + C++ nodes; fusion tracker → **FCW** and lane-departure-style warnings; optional **Foxglove**; YAML/launch config.

**CarOSMini**

**Stack:** Kotlin, Android Automotive, AIDL, Room, Gradle  

Multi-app AAOS infotainment; profile switching via Bluetooth ACL events.

- **IProfileService**, **IPhoneConnectionService**, **Room** persistence; **ACTION_ACL_CONNECTED** → MAC → profile broadcast; documented AAOS + phone emulator workflow.

**Distributed File Sync Engine**

**Stack:** C++17, gRPC, CMake, Protobuf  

C++17 + gRPC bootstrap for bidirectional directory sync; logs and metrics.

- **CMake** + proto RPC surface; structured logging, metrics CSVs, clean shutdown; **CI on Ubuntu 24.04**; roadmap: Merkle/delta/inotify/conflicts.

---

## 📬 How to reach me

| Channel | Detail |
|--------|--------|
| ✉️ **Email** | [sumedhau@usc.edu](mailto:sumedhau@usc.edu) |
| 💼 **LinkedIn** | [linkedin.com/in/SumedhaUmeshKulkarni](https://www.linkedin.com/in/SumedhaUmeshKulkarni/) |
| 🌐 **Portfolio** | [sumedhak.netlify.app](https://sumedhak.netlify.app) |

You can also use this **one-line bio** for your GitHub profile settings (under ~160 characters):

> Full-stack: MS CS @ USC · Embedded (C++/RTOS/Zephyr) · ROS 2 · AAOS/Kotlin · RAG & agents (Haystack, LangGraph) · Python/C++ — open to roles.

*(Alternative, embedded-heavy: C++/RTOS/Zephyr · ROS 2 · Android Automotive · On-device LLMs & tools · RAG pipelines — MS CS @ USC, ex Mercedes-Benz SWE.)*

---

Thanks for visiting 🙏
