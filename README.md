### Hi there 👋.

I am currently building **[Chaos Proxy](https://github.com/Rohith-JN/chaos-proxy)**, a high-performance Chaos Engineering Reverse Proxy designed to help developers build resilient applications.

**The Problem:** simulating poor network conditions (like 3G or flaky Wi-Fi) and protocol failures is often hard to do locally during development.

**The Solution:** A "Man-in-the-Middle" proxy that sits between your frontend and backend, allowing you to inject latency, throttle bandwidth, and tamper with HTTP headers in real-time.

**Technical Highlights:**
* **Core Engine (Go):** Built a custom `ThrottledReadCloser` that wraps standard IO streams to manipulate data flow at the byte level.
* **Concurrency:** Utilizes `sync.RWMutex` for thread-safe, hot-swappable configuration without restarting the server.
* **Dashboard (React + TS):** A "Cockpit" style UI for real-time control and traffic monitoring via a sidecar Admin API.

## Preview
<img width="1920" height="870" alt="{258E7F26-0566-4479-9931-65B279E4261F}" src="https://github.com/user-attachments/assets/69312f09-2ee8-426e-8029-d1a428754ad4" />
