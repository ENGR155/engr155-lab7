# Graph Report - engr155-lab7  (2026-10-23)

## Corpus Check
- 79 files · ~2,893,987 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 35 file(s) not represented in the graph (top: .d 11, .o 11, .s 3)

## Summary
- 1067 nodes · 2442 edges · 32 communities (25 shown, 7 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 134 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `c6902478`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- cmsis_gcc.h
- cmsis_armclang_ltm.h
- core_cm4.h
- cmsis_armclang.h
- cmsis_iccarm.h
- __DSB
- core_cm55.h
- core_armv81mml.h
- core_armv8mml.h
- core_cm33.h
- core_cm35p.h
- core_armv8mbl.h
- core_cm23.h
- cmsis_compiler.h
- cmsis_armcc.h
- core_cm3.h
- core_cm7.h
- core_sc300.h
- core_cm0.h
- core_cm0plus.h
- core_sc000.h
- pmu_armv8.h
- aes_starter.sv
- __PACKED_STRUCT
- __PACKED_STRUCT
- aes_core_tb.sv
- aes_spi_tb.sv
- T_UINT32
- T_UINT32
- README.md

## God Nodes (most connected - your core abstractions)
1. `__DSB()` - 72 edges
2. `__ISB()` - 49 edges
3. `__DMB()` - 8 edges
4. `gpioPinToBase()` - 8 edges
5. `ARM_MPU_LoadEx()` - 7 edges
6. `pinMode()` - 6 edges
7. `digitalWrite()` - 6 edges
8. `main()` - 6 edges
9. `__NVIC_DisableIRQ()` - 5 edges
10. `__NVIC_DisableIRQ()` - 5 edges

## Surprising Connections (you probably didn't know these)
- `__NVIC_SystemReset()` --calls--> `__DSB()`  [INFERRED]
  lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/core_armv8mbl.h → lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/cmsis_gcc.h
- `__NVIC_SystemReset()` --calls--> `__DSB()`  [INFERRED]
  lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/core_armv8mml.h → lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/cmsis_gcc.h
- `__NVIC_SystemReset()` --calls--> `__DSB()`  [INFERRED]
  lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/core_cm0.h → lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/cmsis_gcc.h
- `__NVIC_SystemReset()` --calls--> `__DSB()`  [INFERRED]
  lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/core_cm0plus.h → lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/cmsis_gcc.h
- `__NVIC_SystemReset()` --calls--> `__DSB()`  [INFERRED]
  lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/core_cm1.h → lab07_mcu/lab07_proj/CMSIS_5/CMSIS/Core/Include/cmsis_gcc.h

## Import Cycles
- None detected.

## Communities (32 total, 7 thin omitted)

### Community 0 - "cmsis_gcc.h"
Cohesion: 0.03
Nodes (134): __CLREX(), __CLZ(), __cmsis_start(), __disable_fault_irq(), __disable_irq(), __enable_fault_irq(), __enable_irq(), __get_APSR() (+126 more)

### Community 1 - "cmsis_armclang_ltm.h"
Cohesion: 0.04
Nodes (109): __CLZ(), __get_APSR(), __get_BASEPRI(), __get_CONTROL(), __get_FAULTMASK(), __get_IPSR(), __get_MSP(), __get_MSPLIM() (+101 more)

### Community 2 - "core_cm4.h"
Cohesion: 0.05
Nodes (45): ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ(), NVIC_EncodePriority() (+37 more)

### Community 3 - "cmsis_armclang.h"
Cohesion: 0.06
Nodes (62): __CLZ(), __get_APSR(), __get_BASEPRI(), __get_CONTROL(), __get_FAULTMASK(), __get_IPSR(), __get_MSP(), __get_MSPLIM() (+54 more)

### Community 4 - "cmsis_iccarm.h"
Cohesion: 0.07
Nodes (49): __CLZ(), __get_APSR(), __get_MSPLIM(), __get_PSPLIM(), __iar_u32(), __iar_uint16_read(), __iar_uint16_write(), __iar_uint32_read() (+41 more)

### Community 5 - "__DSB"
Cohesion: 0.11
Nodes (41): SCB_CleanDCache(), SCB_CleanDCache_by_Addr(), SCB_CleanInvalidateDCache(), SCB_CleanInvalidateDCache_by_Addr(), SCB_DisableDCache(), SCB_DisableICache(), SCB_EnableDCache(), SCB_EnableICache() (+33 more)

### Community 6 - "core_cm55.h"
Cohesion: 0.10
Nodes (45): DCB_GetAuthCtrl(), DCB_SetAuthCtrl(), DIB_GetAuthStatus(), ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_ClearTargetState() (+37 more)

### Community 7 - "core_armv81mml.h"
Cohesion: 0.10
Nodes (44): DCB_GetAuthCtrl(), DCB_SetAuthCtrl(), DIB_GetAuthStatus(), ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_ClearTargetState() (+36 more)

### Community 8 - "core_armv8mml.h"
Cohesion: 0.10
Nodes (44): DCB_GetAuthCtrl(), DCB_SetAuthCtrl(), DIB_GetAuthStatus(), ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_ClearTargetState() (+36 more)

### Community 9 - "core_cm33.h"
Cohesion: 0.10
Nodes (44): DCB_GetAuthCtrl(), DCB_SetAuthCtrl(), DIB_GetAuthStatus(), ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_ClearTargetState() (+36 more)

### Community 10 - "core_cm35p.h"
Cohesion: 0.10
Nodes (44): DCB_GetAuthCtrl(), DCB_SetAuthCtrl(), DIB_GetAuthStatus(), ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_ClearTargetState() (+36 more)

### Community 11 - "core_armv8mbl.h"
Cohesion: 0.12
Nodes (37): DCB_GetAuthCtrl(), DCB_SetAuthCtrl(), DIB_GetAuthStatus(), __NVIC_ClearPendingIRQ(), NVIC_ClearTargetState(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ() (+29 more)

### Community 12 - "core_cm23.h"
Cohesion: 0.12
Nodes (37): DCB_GetAuthCtrl(), DCB_SetAuthCtrl(), DIB_GetAuthStatus(), __NVIC_ClearPendingIRQ(), NVIC_ClearTargetState(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ() (+29 more)

### Community 13 - "cmsis_compiler.h"
Cohesion: 0.14
Nodes (20): T_UINT16_READ(), T_UINT16_WRITE(), T_UINT32(), T_UINT32_READ(), T_UINT32_WRITE(), __NVIC_ClearPendingIRQ(), NVIC_DecodePriority(), __NVIC_DisableIRQ() (+12 more)

### Community 14 - "cmsis_armcc.h"
Cohesion: 0.14
Nodes (21): __get_APSR(), __get_BASEPRI(), __get_CONTROL(), __get_FAULTMASK(), __get_FPSCR(), __get_IPSR(), __get_MSP(), __get_PRIMASK() (+13 more)

### Community 15 - "core_cm3.h"
Cohesion: 0.19
Nodes (21): ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ(), NVIC_EncodePriority() (+13 more)

### Community 16 - "core_cm7.h"
Cohesion: 0.19
Nodes (21): ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ(), NVIC_EncodePriority() (+13 more)

### Community 17 - "core_sc300.h"
Cohesion: 0.19
Nodes (21): ITM_CheckChar(), ITM_ReceiveChar(), ITM_SendChar(), __NVIC_ClearPendingIRQ(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ(), NVIC_EncodePriority() (+13 more)

### Community 18 - "core_cm0.h"
Cohesion: 0.25
Nodes (15): __NVIC_ClearPendingIRQ(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ(), NVIC_EncodePriority(), __NVIC_GetEnableIRQ(), __NVIC_GetPendingIRQ(), __NVIC_GetPriority() (+7 more)

### Community 19 - "core_cm0plus.h"
Cohesion: 0.25
Nodes (15): __NVIC_ClearPendingIRQ(), NVIC_DecodePriority(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ(), NVIC_EncodePriority(), __NVIC_GetEnableIRQ(), __NVIC_GetPendingIRQ(), __NVIC_GetPriority() (+7 more)

### Community 20 - "core_sc000.h"
Cohesion: 0.26
Nodes (13): __NVIC_ClearPendingIRQ(), __NVIC_DisableIRQ(), __NVIC_EnableIRQ(), __NVIC_GetEnableIRQ(), __NVIC_GetPendingIRQ(), __NVIC_GetPriority(), __NVIC_GetVector(), __NVIC_SetPendingIRQ() (+5 more)

### Community 21 - "pmu_armv8.h"
Cohesion: 0.23
Nodes (14): ARM_PMU_CNTR_Disable(), ARM_PMU_CNTR_Enable(), ARM_PMU_CNTR_Increment(), ARM_PMU_CYCCNT_Reset(), ARM_PMU_Disable(), ARM_PMU_Enable(), ARM_PMU_EVCNTR_ALL_Reset(), ARM_PMU_Get_CCNTR() (+6 more)

### Community 22 - "aes_starter.sv"
Cohesion: 0.22
Nodes (9): testbench_aes_sbox, aes, aes_core, aes_spi, galoismult, mixcolumn, mixcolumns, sbox_sync (+1 more)

### Community 23 - "__PACKED_STRUCT"
Cohesion: 0.40
Nodes (4): T_UINT16_READ(), T_UINT16_WRITE(), T_UINT32_READ(), T_UINT32_WRITE()

### Community 24 - "__PACKED_STRUCT"
Cohesion: 0.40
Nodes (4): T_UINT16_READ(), T_UINT16_WRITE(), T_UINT32_READ(), T_UINT32_WRITE()

## Knowledge Gaps
- **9 isolated node(s):** `testbench_aes_core`, `testbench_aes_spi`, `aes`, `aes_spi`, `aes_core` (+4 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 33 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **7 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `__DSB()` connect `__DSB` to `cmsis_gcc.h`, `core_cm4.h`, `core_cm55.h`, `core_armv81mml.h`, `core_armv8mml.h`, `core_cm33.h`, `core_cm35p.h`, `core_armv8mbl.h`, `core_cm23.h`, `cmsis_compiler.h`, `core_cm3.h`, `core_cm7.h`, `core_sc300.h`, `core_cm0.h`, `core_cm0plus.h`, `core_sc000.h`?**
  _High betweenness centrality (0.046) - this node is a cross-community bridge._
- **Are the 70 inferred relationships involving `__DSB()` (e.g. with `SCB_CleanDCache()` and `SCB_CleanDCache_by_Addr()`) actually correct?**
  _`__DSB()` has 70 INFERRED edges - model-reasoned connections that need verification._
- **What connects `testbench_aes_core`, `testbench_aes_spi`, `aes` to the rest of the system?**
  _9 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `cmsis_gcc.h` be split into smaller, more focused modules?**
  _Cohesion score 0.029193899782135078 - nodes in this community are weakly interconnected._
- **Why does `__ISB()` connect `__DSB` to `cmsis_gcc.h`, `core_cm4.h`, `core_cm55.h`, `core_armv81mml.h`, `core_armv8mml.h`, `core_cm33.h`, `core_cm35p.h`, `core_armv8mbl.h`, `core_cm23.h`, `cmsis_compiler.h`, `core_cm3.h`, `core_cm7.h`, `core_sc300.h`, `core_cm0.h`, `core_cm0plus.h`, `core_sc000.h`?**
  _High betweenness centrality (0.027) - this node is a cross-community bridge._
- **Are the 47 inferred relationships involving `__ISB()` (e.g. with `SCB_CleanDCache()` and `SCB_CleanDCache_by_Addr()`) actually correct?**
  _`__ISB()` has 47 INFERRED edges - model-reasoned connections that need verification._
- **Should `cmsis_armclang_ltm.h` be split into smaller, more focused modules?**
  _Cohesion score 0.03570843570843571 - nodes in this community are weakly interconnected._