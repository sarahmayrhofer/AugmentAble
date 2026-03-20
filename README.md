AugmentAble

AugmentAble is a research-oriented web augmentation tool designed to improve web accessibility in real-time. It acts as a non-invasive, client-side layer that identifies and repairs common accessibility violations (WCAG) directly in the browser's Document Object Model (DOM). The project combines traditional heuristic-based remediation with modern Multimodal Large Language Models (LLMs) to bridge the gap between static web content and an inclusive user experience.
Key Features

Heuristic Remediation Engine:
The system performs immediate, rule-based corrections for structural issues. This includes recalculating text colors for WCAG contrast compliance and injecting ARIA attributes based on element metadata and context.

AI-Powered Semantic Analysis:
For complex elements like images without alternative text, the system uses a multimodal pipeline. It transmits image data to inference APIs (e.g., Qwen2.5-VL or Aya-Vision) to generate descriptive labels. The modular architecture is designed to support future integration with locally hosted LLMs to address data privacy concerns.

Audit Interface and Monitoring:
To ensure transparency, the system includes a UI panel that tracks all modifications. A dedicated focus mode allows users to highlight automated fixes with high-visibility outlines, providing immediate feedback on performed improvements.
Installation

    Install the Tampermonkey browser extension.

    Open the AugmentAble.user.js file in this repository.

    Select the Raw view to prompt the installation.

    On the first run, the script will prompt for a HuggingFace API Key, which is stored locally in the browser's secure storage.

Citation

If you use this tool in your research, please cite:

Sarah Mayrhofer, AugmentAble: Leveraging Web Augmentation and Multimodal LLMs for Real-Time Accessibility Remediation (2026).
Disclaimer

This is a research prototype. Data processed via the AI pipeline is sent to the configured inference provider. Ensure your API usage complies with your organization's privacy policies.
