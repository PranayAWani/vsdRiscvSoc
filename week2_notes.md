1. Four Major Sub-Modules in caravel
- padframe
- housekeeping
- management_soc_wrapper
- user_project_wrapper

2. Signals Crossing the "Management Protect" Boundary
- Wishbone bus signals
- IRQ (interrupt) lines
- GPIO signals
- Clock and reset signals
- Power-on-reset and control/status signals

3. Reset and Clock Synchronization Point
- Reset and clock are first synchronized at the entry points of the management_soc_wrapper and user_project_wrapper modules, using standard two-stage synchronizer circuits to ensure safe crossing into the respective clock domains.
