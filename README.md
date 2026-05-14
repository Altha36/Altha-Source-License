# Altha Source License (ASL) v2.0

![ASL-2.0](https://img.shields.io/badge/License-ASL_v2.0-feca74?style=for-the-badge&labelColor=202020)
  
A modern, modular, and competition-aware source-available license.

---

## What is ASL?

The **Altha Source License (ASL)** is a source-available license designed for the modern software economy. It allows developers to share their source code transparently while legally protecting their business model from direct commercial exploitation by competitors.

### Why choose ASL?
*   **Market Defense:** Prevents competitors from "cloning" your service using your own code.
*   **Public Modularity:** The legal text is agnostic. Specific protections are defined by you in a metadata file (`NOTICE.txt`).
*   **Ecosystem Friendly:** Built to coexist with kernels (Linux) and libraries (GPL/MIT) without "license contamination" or compatibility conflicts.
*   **Sustainability:** Enables public auditing and community contributions without sacrificing your commercial viability.

---

## How to implement it in your project

### 1. Include the License
Add the [`LICENSE`](LICENSE.md) file to the root of your repository.

### 2. Define your "Primary Service"
Create a file named `NOTICE.txt` (or similar). This is where you declare the specific niche that is restricted for competitors.

**Example `NOTICE.txt`:**
```text
ALTHA SOURCE LICENSE (ASL) v2.0 - PRIMARY SERVICE DESIGNATION

Project: [Insert Project Name]
Licensor: [Insert Licensor Name or Entity]

Under the terms of the Altha Source License v2.0, the "Primary Service" 
for this Work is specifically designated as the commercial provision, 
sale, distribution, or operation of:

1. [Insert specific restricted niche, e.g., Managed game server hosting]
2. [Insert second specific restriction, e.g., Commercial operating system distributions based on this Work]
3. [Insert third specific restriction or leave blank, e.g., Any commercial cloud platform that directly replicates the Licensor's official product]

Any commercial use that falls WITHIN this designated scope is strictly prohibited 
under Section 4.2 of the ASL v2.0, unless you have obtained a separate, 
explicit Commercial License from the Licensor.

Any commercial use that falls OUTSIDE of this designated scope (including but 
not limited to: deploying the Work for internal business tools, utilizing the Work 
in non-competing commercial products, or educational research) is fully 
permitted under the terms of the ASL v2.0.

For commercial licensing inquiries, contact: [Insert Contact Email or URL]
```

### 3. Identify your Files
Add the SPDX header to the top of your source code files:

```go
// SPDX-License-Identifier: ASL-2.0
// Copyright (c) 2026 [Your Name/Entity]. All rights reserved.
```
Or
```python
# SPDX-License-Identifier: ASL-2.0
# Copyright (c) 2026 [Your Name/Entity]. All rights reserved.
```
