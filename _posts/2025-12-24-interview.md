---
title: interview
author: rainer
date: 2025-12-29 1:26:00 +0300
categories: [5G NR]
tags: [5G NR]
math: true
mermaid: true
render_with_liquid: false
image: 
    path: 
---

I understand the technical point, but to make sure I explain it exactly, may I switch to Vietnamese for this part?


# Mục lục

- [Mục lục](#mục-lục)
- [Introduce some experience that you work with 4/5G Technology.](#introduce-some-experience-that-you-work-with-45g-technology)
- [How the site link to make UE talk to each other.](#how-the-site-link-to-make-ue-talk-to-each-other)
- [What is similarity between the 4G and Wifi System](#what-is-similarity-between-the-4g-and-wifi-system)
- [Followed by the CV, what’s the exactly feature during last 3 years on LTE L3? What is the purpose of that feature, how did you change and how did you do the test?](#followed-by-the-cv-whats-the-exactly-feature-during-last-3-years-on-lte-l3-what-is-the-purpose-of-that-feature-how-did-you-change-and-how-did-you-do-the-test)
- [How the test environment setup?](#how-the-test-environment-setup)
- [Wifi 6, 5G and 4G, compare the pros and cons of each devices, which one is the best?](#wifi-6-5g-and-4g-compare-the-pros-and-cons-of-each-devices-which-one-is-the-best)
- [What kind of application would really need 5G?](#what-kind-of-application-would-really-need-5g)
- [What kind of 4G/5G work have you done?](#what-kind-of-4g5g-work-have-you-done)
- [What projects are you most confident talking about?](#what-projects-are-you-most-confident-talking-about)
- [Explain one project in detail: 5G software upgrade and feature integration](#explain-one-project-in-detail-5g-software-upgrade-and-feature-integration)
- [What exactly did you do in the 5G Multi Band project?](#what-exactly-did-you-do-in-the-5g-multi-band-project)
- [What was the purpose of the UpLink Dynamic project, and what did you change?](#what-was-the-purpose-of-the-uplink-dynamic-project-and-what-did-you-change)
- [Tell me about your CI/CD for L1 project](#tell-me-about-your-cicd-for-l1-project)
- [Tell me about your AI RAN project](#tell-me-about-your-ai-ran-project)
- [How do you describe your technical strengths?](#how-do-you-describe-your-technical-strengths)
- [What exact LTE L3 feature did you work on?](#what-exact-lte-l3-feature-did-you-work-on)
- [11) How do you set up a test environment for your feature?](#11-how-do-you-set-up-a-test-environment-for-your-feature)
  - [Trả lời tiếng Việt](#trả-lời-tiếng-việt)
  - [English answer](#english-answer)
- [12) What is the most difficult technical issue you faced?](#12-what-is-the-most-difficult-technical-issue-you-faced)
  - [Trả lời tiếng Việt](#trả-lời-tiếng-việt-1)
  - [English answer](#english-answer-1)
- [13) How do you explain O-RAN / FAPI / L1 knowledge in interview?](#13-how-do-you-explain-o-ran--fapi--l1-knowledge-in-interview)
  - [Trả lời tiếng Việt](#trả-lời-tiếng-việt-2)
  - [English answer](#english-answer-2)
- [14) Compare 4G, 5G, and Wi-Fi 6](#14-compare-4g-5g-and-wi-fi-6)
  - [Trả lời tiếng Việt](#trả-lời-tiếng-việt-3)
  - [English answer](#english-answer-3)
- [15) What kind of applications really need 5G?](#15-what-kind-of-applications-really-need-5g)
  - [Trả lời tiếng Việt](#trả-lời-tiếng-việt-4)
  - [English answer](#english-answer-4)
- [16) How do you answer “Why should we hire you?”](#16-how-do-you-answer-why-should-we-hire-you)
  - [Trả lời tiếng Việt](#trả-lời-tiếng-việt-5)
  - [English answer](#english-answer-5)


---

<a id="introduce-some-experience-that-you-work-with-4-5g-technology"></a>

# Introduce some experience that you work with 4/5G Technology.

I am a telecom software engineer currently working on 5G embedded systems, with strong focus on Layer 1, software integration, low-level Linux, debugging, and validation. My work has involved developing and integrating features for 4G/5G systems, especially in areas such as software release upgrade, integration of new framework-supported features, performance optimization, runtime issue analysis, and system stabilization after integration.

My strength is not only writing or modifying code, but also tracing issues across multiple layers of the system, from build flow, runtime behavior to interface integration and lab validation. I can use  VSG(N5182B)/VSA()  instrument from keysight. I am comfortable working with C/C++, Linux, DPDK, GDB, Makefile, Git/GitLab, Jenkins, and 5G PHY channel PDSCH, PUSCH, PDCCH, PUCCH PRACH SSB, DMRS, CSI-RS

<a id="how-the-site-link-to-make-ue-talk-to-each-other"></a>

# How the site link to make UE talk to each other.

Two UEs do not talk to each other directly in a normal cellular architecture. Their traffic is controlled and forwarded by the network.

In 4G, the packet typically goes from UE to eNB, then through the transport network to the EPC, and then back toward the destination UE through the serving eNB.

In 5G, the same idea applies, but the user plane is handled through the 5G core, especially the UPF.

So the “site link” is not just a radio link. It includes radio access, transport/backhaul, core routing, and the return path to the destination UE.

The radio side provides access, but the actual UE-to-UE communication depends on end-to-end user-plane routing,  and core-network forwarding

<a id="what-is-similarity-between-the-4g-and-wifi-system"></a>

# What is similarity between the 4G and Wifi System

4G and Wi-Fi are both wireless communication systems, so they share many common concepts such as modulation, coding, MIMO, OFDM-based transmission, channel estimation, and medium access control.

However, 4G is a cellular system designed for wide-area mobility, controlled resource allocation, and operator-managed QoS, while Wi-Fi is mainly a local-area system optimized for shorter-range access with a different MAC.

<a id="followed-by-the-cv-what-s-the-exactly-feature-during-last-3-years-on-lte-l3-what-is-the-purpose-of-that-feature-how-did-you-change-and-how-did-you-do-the-test"></a>

# Followed by the CV, what’s the exactly feature during last 3 years on LTE L3? What is the purpose of that feature, how did you change and how did you do the test?

<a id="how-the-test-environment-setup"></a>

# How the test environment setup?

The test environment usually included the DUT software running on the target platform, UE or UE simulator, and logging/monitoring components.

Depending on the scenario, we also used RF attenuation, packet capture, system logs, and KPI collection to validate both protocol behavior and performance.

* **Radio side**: eNB/gNB, UE hoặc UE simulator
* **Core side**: EPC/5GC test environment
* **Transport side**: switch/VLAN/IP routing
* **Traffic side**: iperf, ping, throughput tools
* **Debug side**:

  * Wireshark / tcpdump
  * internal logs
  * crash dump
  * KPI counters

<a id="wifi-6-5g-and-4g-compare-the-pros-and-cons-of-each-devices-which-one-is-the-best"></a>

# Wifi 6, 5G and 4G, compare the pros and cons of each devices, which one is the best?

I would not say one is universally the best.

4G is mature, stable, and cost-effective for broad coverage.

5G is better when you need higher capacity, lower latency, and more advanced service capability.

Wi-Fi 6 is very strong for indoor, local, high-throughput access with relatively low deployment cost.

So the best technology depends on the use case: public mobility and operator-managed service usually favor cellular, while local indoor access often favors Wi-Fi.

<a id="what-kind-of-application-would-really-need-5g"></a>

# What kind of application would really need 5G?

Applications that truly benefit from 5G are those requiring either much higher capacity, lower latency, better mobility support, or higher device density than 4G can provide.

Examples include industrial automation, private wireless networks, AR/VR, cloud gaming, smart manufacturing, and large-scale IoT deployments.

5G becomes valuable when the requirement is not just “internet access,” but performance, scale, and service differentiation.

<a id="what-kind-of-4g-5g-work-have-you-done"></a>

# What kind of 4G/5G work have you done?

My 4G/5G experience is mainly on the software and system-integration side rather than RF planning or field deployment. I have participated in research and development of Layer 1 features for 4G/5G networks, and I have worked on software upgrade, feature integration, uplink processing enhancement, multi-band support, CI/CD automation for L1, and more recently AI RAN optimization on target hardware.

My responsibilities typically include analyzing the impact of a new feature or release, modifying or integrating software, resolving build/runtime/integration issues, debugging on Linux platform, and then validating the behavior through controlled lab testing.

<a id="what-projects-are-you-most-confident-talking-about"></a>

# What projects are you most confident talking about?

I am most confident discussing five main projects.

The first is **5G software upgrade and feature integration**. It is very close to real integration work because it requires analyzing differences between the current and newer vendor releases, merging newly supported framework features, migrating to newer DPDK versions, and resolving compatibility, build, runtime, and stability issues after the upgrade.

The second is **5G Multi Band**, where I updated software modules to support multiple band configurations, resolved issues during integration, and supported validation, including testing with VSA/VSG waveform instruments.

The third is **UpLink Dynamic**, where I worked on integrating the dynamic uplink feature, updating feature parameters, control logic, and software flow, while resolving runtime and integration issues and stabilizing the software.

The fourth is **CI/CD for L1**, where I analyzed the existing workflow, built automation pipelines for build/integration/validation, automated source sync, build, script execution, log collection, artifact handling, and fixed pipeline failures.

The fifth is **AI RAN**, where I optimized code and processing flow to improve latency, throughput, memory usage, and resource efficiency for model execution on Linux-based target hardware.

<a id="explain-one-project-in-detail-5g-software-upgrade-and-feature-integration"></a>

# Explain one project in detail: 5G software upgrade and feature integration

In this project, the main objective was to upgrade the 5G software to newer vendor releases, integrate newly supported framework features, and migrate to newer DPDK versions. 

My role was to analyze the differences between the old and new releases, evaluate software impact, merge new features into the current codebase, fix build and compatibility issues, resolve integration problems, and support validation after the upgrade. My contribution was to make sure the system was not only buildable on the new baseline, but also stable and usable after migration

For example, when a new feature requires an additional configuration from L2, that feature could affect the all system.

The challenge was not just replacing versions, but ensuring compatibility, stability, and successful system integration after the upgrade. and debugging tools (GDB) can not used on low-latency real-time threads.

<a id="what-exactly-did-you-do-in-the-5g-multi-band-project"></a>

# What exactly did you do in the 5G Multi Band project?

In the 5G Multi Band project, the target was to extend the existing software platform to support multi band configurations. My work included develop and integrating the software modules to enable multi-band operation, and then resolving build, runtime, and integration issues that during deployment.

Besides coding and integration, I also supported debugging, validation, and stability improvement during Multi Band operation. This project also involved testing with VSA/VSG instruments, so I gained additional experience in validating system behavior from waveform measurement perspective, not only from software logs

The challenge is not only to develop and test, but also to integrate with multiple vendor RUs. 

<a id="what-was-the-purpose-of-the-uplink-dynamic-project-and-what-did-you-change"></a>

# What was the purpose of the UpLink Dynamic project, and what did you change?

The purpose of the UpLink Dynamic project was to improve the flexibility and save resources of uplink processing in the existing 5G software platform. I develop the CP/UP packet flow to follow the exact L2 scheduling, instead of transmitting the full resource grid. Then close the ORAN packet and send to RU. Beside, I also support measurement and testing with VSG instrument (N5182B).

The challenge is not only developing and testing, but also requiring the Resource Unit (RU) to support the feature. For example, when I send the RB configuration via L2 to the RU, the RU still handles the all resource grid. So, I have to support the RU in developing the feature using the ORAN packet that the DU sends to the RU. 

<a id="tell-me-about-your-ci-cd-for-l1-project"></a>

# Tell me about your CI/CD for L1 project

CI/CD for L1 is an important project because it shows that I do not only work on feature code, but also on improving development efficiency and software quality. The objective was to automate the build, integration, validation, and delivery workflow for 5G L1 software.

My role was to analyze the existing development workflow, design and develop CI/CD pipelines for build/integration/validation, automate source sync, build execution, script running, log collection, and artifact handling. I also investigated and fixed pipeline failures, build issues, and environment-related problems. The main value of this project was reducing integration time, minimizing manual errors, and making software validation more repeatable and stable

The challenge lies in handling logs for multiple channels. Therefore, I reduced it to a text processing problem and returned the pass/fail result at the end of the stage. and debugging tools (GDB) can not used on low-latency real-time threads.


<a id="tell-me-about-your-ai-ran-project"></a>

# Tell me about your AI RAN project

AI RAN is a project that applies AI to the PUSCH channel. My work mainly focus is model execution performance on target hardware. The target  was to improve latency, throughput, resource efficiency, and system integration of AI RAN software on Linux platform.

In this project, I analyzed performance bottlenecks affecting model execution on the target hardware, optimized software code and processing flow to improve latency and throughput, and improved memory usage, data handling, and resource efficiency. This project shows that I am not limited to traditional telecom feature work, but can also handle performance tuning from a system-level perspective.

---

For CPU-side optimization, I focused on reducing unnecessary operations in hot paths, minimizing branch-heavy logic such as too many IF statements inside hot loops, and improving execution efficiency.

For memory-side optimization, I worked on better data layout, alignment, memory access patterns, and reducing unnecessary memory copies to improve cache efficiency.

For example: storing a 2D array in memory using row-major allows each cache line to utilize more useful bytes. Or, use a variable have size matches the word size of CPU.

The challenge was not only in development and testing, but also in making sure no unexpected process was using CPU cores when the AI workload was running. I  manage task allocation, and debugging tools (GDB) can not used on low-latency real-time threads.

<a id="how-do-you-describe-your-technical-strengths"></a>

# How do you describe your technical strengths?

My strongest technical point is working in complex telecom software environments where the issue is not isolated to a single module. I am comfortable with cross-layer problems, especially those involving build flow, runtime behavior, timing, integration, platform behavior, performance, or stability.

I also have a solid Embedded Linux background, including C/C++ on Linux, process/thread, IPC, memory management, file system, socket programming, TCP/UDP, Makefile, build automation, GDB, Valgrind, and Git/GitLab. In addition, I have basic knowledge of U-Boot, kernel, rootfs, Linux device drivers, and register-level understanding. On the telecom side, my CV also reflects understanding of 5G RAN/O-RAN, Open Fronthaul, High-PHY/Low-PHY split, FAPI/nFAPI, and 5G NR physical channels and signals.

<a id="what-exact-lte-l3-feature-did-you-work-on"></a>

# What exact LTE L3 feature did you work on?

I want to be transparent that my recent experience is stronger in 5G L1 software, integration, low-level Linux, and system troubleshooting than in pure LTE L3 feature ownership. However, I work well in cross-layer environments where higher-layer behavior directly affects integration flow, runtime behavior, and system validation.

<a id="11-how-do-you-set-up-a-test-environment-for-your-feature"></a>

# 11) How do you set up a test environment for your feature?

## Trả lời tiếng Việt

Môi trường test của tôi thường gồm nhiều phần: software chạy trên Linux target platform, cấu hình feature cần xác nhận, các thành phần integration liên quan, hệ thống thu thập log, script test hoặc validation flow, và nếu cần thì có thêm thiết bị đo hoặc môi trường lab phục vụ xác nhận hành vi radio.

Tôi thường quan tâm không chỉ đến việc “test pass”, mà còn đến khả năng tái hiện và debug được vấn đề. Vì vậy khi setup test environment, tôi chú ý tới khả năng so sánh baseline trước và sau khi thay đổi, khả năng gom log đầy đủ, cách cô lập biến số và nếu liên quan đến waveform/measuring side thì có thể dùng VSA/VSG như trong project Multi Band. Trong pipeline side, tôi cũng quen với việc tự động hóa build, run script, log collection và artifact handling để việc validation có tính lặp lại tốt hơn.

## English answer

My test environment usually includes the software running on Linux target platform, the feature configuration to be validated, the related integration components, log collection system, test scripts or validation flow, and when needed, lab instruments or radio-related setup for behavior verification.

I do not only focus on making the test pass, but also on making the issue reproducible and debuggable. So when I set up a test environment, I pay attention to baseline-versus-changed comparison, complete log collection, variable isolation, and if waveform-related validation is needed, using tools such as VSA/VSG as in the Multi Band project. On the pipeline side, I am also used to automating build, script execution, log collection, and artifact handling to make validation more repeatable.

---

<a id="12-what-is-the-most-difficult-technical-issue-you-faced"></a>

# 12) What is the most difficult technical issue you faced?

## Trả lời tiếng Việt

Một trong những tình huống kỹ thuật khó nhất với tôi thường là các lỗi runtime hoặc integration chỉ xuất hiện trong một điều kiện rất cụ thể, không dễ tái hiện ổn định, trong khi triệu chứng lại nằm ở một chỗ nhưng root cause nằm ở chỗ khác. Với kiểu lỗi này, phần khó nhất không phải chỉ là sửa code, mà là phải biến một vấn đề mơ hồ thành thứ có thể tái hiện, có log, có bằng chứng và có đường hướng phân tích rõ ràng.

Cách tôi xử lý thường là thu hẹp phạm vi từng bước: so sánh baseline trước và sau thay đổi, xem lại build/config/runtime condition, phân tích log, dùng GDB hoặc các công cụ debug phù hợp, rồi xác minh lại bằng test có kiểm soát. Đây cũng là kiểu việc rất sát với các project của tôi như release upgrade, feature integration, CI/CD failure investigation hay performance tuning trên Linux.

## English answer

One of the most difficult technical situations for me is usually a runtime or integration issue that appears only under specific conditions, is not easy to reproduce consistently, and where the visible symptom is not the actual root cause. In this kind of problem, the hardest part is not just fixing code, but turning a vague issue into something reproducible, evidence-based, and technically structured.

My usual approach is to narrow the scope step by step: compare baseline before and after the change, review build/config/runtime conditions, analyze logs, use GDB or other suitable debugging tools, and then verify the conclusion through controlled testing. This kind of work is very close to the type of projects I have done, such as release upgrade, feature integration, CI/CD failure investigation, and performance tuning on Linux.

---

<a id="13-how-do-you-explain-o-ran-fapi-l1-knowledge-in-interview"></a>

# 13) How do you explain O-RAN / FAPI / L1 knowledge in interview?

## Trả lời tiếng Việt

Nếu interviewer hỏi sâu về 5G architecture, tôi sẽ trả lời rằng tôi có nền tảng tốt về 5G RAN và O-RAN architecture, đặc biệt là các khái niệm như RU/DU disaggregation, open interface principles, Open Fronthaul, và High-PHY/Low-PHY split. Tôi cũng quen với việc nhìn hệ thống theo hướng MAC–PHY interaction thông qua FAPI và nFAPI, và hiểu kiến trúc xử lý L1 cũng như các kênh tín hiệu chính như PDSCH, PUSCH, PDCCH, PUCCH, PRACH, SSB, DMRS, CSI-RS.

Điểm cần nhấn mạnh là tôi không chỉ biết lý thuyết khái niệm, mà còn làm việc trong môi trường 5G L1 software thực tế, nên khi nhìn một feature hay một issue tôi sẽ nhìn nó theo hướng data flow, interface impact, timing và integration chứ không chỉ định nghĩa lý thuyết.

## English answer

If the interviewer asks about 5G architecture, I would say that I have a solid foundation in 5G RAN and O-RAN architecture, especially concepts such as RU/DU disaggregation, open interface principles, Open Fronthaul, and High-PHY/Low-PHY split. I am also familiar with MAC–PHY interaction through FAPI and nFAPI, and I understand L1 processing architecture as well as key physical channels and signals such as PDSCH, PUSCH, PDCCH, PUCCH, PRACH, SSB, DMRS, and CSI-RS.

The important point is that I do not only know the concepts theoretically. I work in a real 5G L1 software environment, so when I look at a feature or an issue, I naturally think in terms of data flow, interface impact, timing, and system integration, not only definitions.

---

<a id="14-compare-4g-5g-and-wi-fi-6"></a>

# 14) Compare 4G, 5G, and Wi-Fi 6

## Trả lời tiếng Việt

Tôi sẽ không nói công nghệ nào tốt nhất tuyệt đối, vì còn phụ thuộc use case. 4G mạnh ở độ trưởng thành, vùng phủ rộng và chi phí triển khai hợp lý hơn. 5G mạnh hơn khi cần throughput cao hơn, latency thấp hơn, dung lượng lớn hơn và hỗ trợ các dịch vụ nâng cao hơn. Wi-Fi 6 lại rất phù hợp cho môi trường indoor/local-area, throughput cao và chi phí triển khai thấp hơn trong nhiều trường hợp.

Nếu cần chọn theo bài toán, tôi sẽ nói: với public mobility và service diện rộng có quản lý thì cellular mạnh hơn; với truy cập cục bộ trong nhà thì Wi-Fi thường là lựa chọn kinh tế và phù hợp hơn; còn 5G phát huy rõ nhất khi bài toán yêu cầu hiệu năng, độ trễ, mật độ thiết bị hoặc khả năng kiểm soát dịch vụ ở mức cao. Phần nền kiến thức 4G/5G architecture trong CV của tôi giúp tôi nhìn câu hỏi này theo góc hệ thống chứ không trả lời theo kiểu marketing.

## English answer

I would not say one technology is always the best, because it depends on the use case. 4G is strong in maturity, broad coverage, and more low deployment cost. 5G is better when higher throughput, lower latency, larger capacity, and more advanced service capability are needed. Wi-Fi 6 is very suitable for indoor or local-area environments, with high throughput and lower deployment cost in many cases.

If I need to choose by scenario, I would say: for public mobility and managed wide-area service, cellular is stronger; for local indoor access, Wi-Fi is often the more practical and cost-effective choice; and 5G becomes most valuable when the requirement is performance, low latency, high device density, or stronger service control. My 4G/5G architecture background helps me answer this from a system perspective rather than a marketing perspective.

---

<a id="15-what-kind-of-applications-really-need-5g"></a>

# 15) What kind of applications really need 5G?

## Trả lời tiếng Việt

Những ứng dụng thực sự cần 5G thường là các ứng dụng đòi hỏi nhiều hơn mức “truy cập internet bình thường”, ví dụ cần throughput cao, latency thấp, mật độ thiết bị lớn, mobility tốt hoặc QoS được kiểm soát rõ ràng. Ví dụ là industrial automation, private wireless network, cloud gaming, AR/VR, edge AI use case, hoặc các hệ thống cần truyền dữ liệu lớn với độ ổn định và hiệu năng cao.

Với background của tôi ở 5G software, tôi nhìn 5G không chỉ là tốc độ cao hơn, mà là một nền tảng hỗ trợ các bài toán mà 4G hoặc Wi-Fi trong nhiều trường hợp khó đáp ứng đồng thời tất cả các yêu cầu về bandwidth, latency, stability và service control.

## English answer

Applications that truly need 5G are those that require more than normal internet access, for example high throughput, low latency, high device density, good mobility, or stronger QoS control. Examples include industrial automation, private wireless networks, cloud gaming, AR/VR, edge AI use cases, and systems that require large data transfer with strong stability and performance.

With my 5G software background, I see 5G not just as “higher speed”, but as a platform that supports scenarios where 4G or Wi-Fi may struggle to meet bandwidth, latency, stability, and service control requirements at the same time.

---

<a id="16-how-do-you-answer-why-should-we-hire-you"></a>

# 16) How do you answer “Why should we hire you?”

## Trả lời tiếng Việt

Nếu team cần một kỹ sư làm tốt trong môi trường phần mềm viễn thông phức tạp, đặc biệt ở các bài toán 5G software integration, low-level Linux, performance, debugging và validation, thì tôi nghĩ tôi là người phù hợp. Tôi có nền tảng kỹ thuật khá sát với môi trường thực tế: C/C++, Linux, DPDK, GDB, CI/CD, integration, và kiến thức hệ thống về 5G RAN/O-RAN/L1.

Điểm khác biệt của tôi là tôi không nhìn vấn đề theo kiểu một module đơn lẻ. Tôi quen với việc biến một lỗi khó hoặc một task integration phức tạp thành bài toán kỹ thuật có cấu trúc, có thể phân tích, có thể debug và có thể xác nhận được bằng test. Những project trong CV của tôi cũng phản ánh khá rõ hướng đóng góp này.

## English answer

If the team needs an engineer who can work effectively in complex telecom software environments, especially on 5G software integration, low-level Linux, performance, debugging, and validation, then I believe I am a strong fit. I have a technical foundation that is close to real development environments: C/C++, Linux, DPDK, GDB, CI/CD, integration, and system knowledge of 5G RAN/O-RAN/L1.

What differentiates me is that I do not look at problems as isolated module-level issues. I am used to turning difficult bugs or complex integration tasks into structured engineering problems that can be analyzed, debugged, and validated through controlled testing. The projects in my CV reflect that contribution quite clearly.

I understand the technical point, but to make sure I explain it accurately, may I switch to Vietnamese for this part?

