## 2024-12-26 - [Lazy Loading Large Models]
**Learning:** Initializing heavy resources (like LLMs or ML pipelines) in `__init__` kills startup performance and wastes resources if those capabilities aren't always used.
**Action:** Use lazy loading patterns (init to None, load on first use) for any resource > 50MB or requiring network calls.
