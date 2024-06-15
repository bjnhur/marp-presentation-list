---
marp: true
theme: gaia
title: test
header: test
paginate: true
---

![bg right](https://images.unsplash.com/photo-1569156132115-c734e2fc040c?crop=entropy&cs=srgb&fm=jpg&ixid=M3w1NTU5NjN8MHwxfHNlYXJjaHw5fHx1dm18ZW58MHwxfHx8MTcxODQ0Mjk1Nnww&ixlib=rb-4.0.3&q=85)

# UVM Basic
Presenter: [Your Name]

---

# Introduction to UVM
- Universal Verification Methodology
- Advanced verification methodology
- Based on SystemVerilog

<!-- In this slide, I will introduce what UVM is and its basis on SystemVerilog. -->

---

# Why UVM?
- Increases productivity
- Improves reusability
- Enhances modularity
- Facilitates team-based verification

<!-- Here, I will explain the benefits of using UVM, including productivity, reusability, modularity, and team-based verification. -->

---

# UVM Components
- UVM Test
- UVM Environment
- UVM Agent
- UVM Sequencer
- UVM Driver
- UVM Monitor

<!-- In this slide, I will discuss the different components of UVM. -->

---

# UVM Test
- Top-level component
- Controls the execution of the test

```systemverilog
class my_test extends uvm_test;
  `uvm_component_utils(my_test)
  ...
endclass
```

<!-- I will explain what UVM Test is and show an example code of UVM Test. -->

---

# UVM Environment
- Contains and controls UVM Agents
- Connects to DUT (Device Under Test)

```systemverilog
class my_env extends uvm_env;
  `uvm_component_utils(my_env)
  ...
endclass
```

<!-- I will explain what UVM Environment is and show an example code of UVM Environment. -->

---

# UVM Agent
- Contains and controls UVM Sequencer, UVM Driver, and UVM Monitor
- Connects to DUT interface

```systemverilog
class my_agent extends uvm_agent;
  `uvm_component_utils(my_agent)
  ...
endclass
```

<!-- I will explain what UVM Agent is and show an example code of UVM Agent. -->

---

# UVM Sequencer
- Generates and randomizes sequences
- Sends sequences to UVM Driver

```systemverilog
class my_sequencer extends uvm_sequencer;
  `uvm_component_utils(my_sequencer)
  ...
endclass
```

<!-- I will explain what UVM Sequencer is and show an example code of UVM Sequencer. -->

---

# UVM Driver
- Receives sequences from UVM Sequencer
- Drives DUT interface

```systemverilog
class my_driver extends uvm_driver;
  `uvm_component_utils(my_driver)
  ...
endclass
```

<!-- I will explain what UVM Driver is and show an example code of UVM Driver. -->

---

# UVM Monitor
- Observes DUT interface
- Collects coverage and transaction data

```systemverilog
class my_monitor extends uvm_monitor;
  `uvm_component_utils(my_monitor)
  ...
endclass
```

<!-- I will explain what UVM Monitor is and show an example code of UVM Monitor. -->

---

# Conclusion
- UVM is a powerful verification methodology
- It improves productivity and reusability
- It enhances modularity and facilitates team-based verification

<!-- In the final slide, I will summarize the key points of the presentation. -->
