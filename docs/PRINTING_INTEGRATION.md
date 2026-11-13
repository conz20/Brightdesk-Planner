# Brightdesk Planner printing integration

Planner uses the canonical dependency-free Brightdesk Printing adapter snapshot. The Electron main process owns a sender-authorized IPC bridge for queue listing, network discovery, user-selected WSD pairing, capabilities, native settings and print submission. Renderer access is limited to the context-isolated preload API.

**Customer-facing UI boundary:** the renderer currently connects only queue listing, Print and Printer settings. Network discovery, user-approved WSD pairing and capability lookup are exposed through protected IPC/preload APIs but are not wired to a customer-facing screen. Users must add the printer through operating-system settings before it becomes a usable queue.

The native build script runs after the Rust Node-API build. macOS builds a universal Bonjour/IPP helper; Windows builds the IPP/WSD helper using Visual Studio C++ Build Tools and Windows SDK; Linux uses the host CUPS `ippfind` utility. Installer configuration unpacks the native helpers and Rust module outside ASAR.

Print submission uses the visible OS print dialog. Discovery does not create queues or install drivers. Submission acceptance does not confirm a physical page was printed. Virtual-printer tests are not hardware verification.
