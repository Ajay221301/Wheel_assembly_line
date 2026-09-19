#  Operations Industrial Engineer Project

## Project Overview

This project is based on the **Operations Industrial Engineer** job simulation from **Siemens Mobility – Project Velocity**, focused on improving the manufacturing process for the **Aurora Express high-speed train**.

The project involved analyzing a **wheel assembly time study**, identifying a bottleneck, and then proposing a practical **assembly-line layout improvement** to reduce the impact of the bottleneck.

The main objective was to improve production flow and efficiency while considering practical constraints such as **cost, implementation time, production disruption, and existing resources**.

---

## Business Problem

The wheel assembly section contained a process bottleneck that was increasing the time required to complete the wheel assembly process.

The initial improvement idea was to automate the bottleneck using a customized robotic system. However, the proposed automation was not feasible because:

- A customized robot would be required.
- The investment cost was considered too high.
- Development would take more than one year.
- The project needed a solution that could be implemented sooner.

Therefore, the focus shifted from full automation to **layout and workflow improvement using existing resources**.

---

# Task 1 – Time Study and Bottleneck Identification

## Objective

The first task was to analyze the wheel assembly time-study data and identify the process step contributing most to the delay.

### Approach

The analysis followed these steps:

1. Reviewed the wheel assembly process and its individual tasks.
2. Examined the time taken by different process steps.
3. Compared the duration and variation of the tasks.
4. Identified the longest-duration operation as the key bottleneck in the simulation.
5. Considered possible operational factors such as task complexity, equipment usage, and operator movement.
6. Proposed an initial improvement through automation.

### Bottleneck

**Step 14 – Wheel mounting / wheel press operation** was identified as the key bottleneck based on the time-study analysis.

The important distinction is:

> The time-study data identifies **where the bottleneck occurs**. Additional process and layout analysis is required to understand **what factors contribute to the delay**.

### Initial Improvement Idea

The initial proposal was to use a **customized automated wheel-mounting system**.

However, this solution was rejected as impractical because of its high cost and long development time.

This led to the second task: redesigning the layout using existing resources.

---

# Task 2 – Assembly Layout Reconfiguration

## Objective

The objective was to redesign the wheel assembly layout to reduce unnecessary:

- Material movement
- Worker movement
- Setup time
- Waiting
- Handling
- Workstation congestion

The redesign had to use the **existing resources** instead of relying on the expensive customized robot.

---

## Original Layout

The original layout contains:

- Wheel Press
- Crane
- Four assembly areas
- Warehouse
- Shared material-flow paths

(<img width="2032" height="1170" alt="original_layout" src="https://github.com/user-attachments/assets/b2eaeecb-13dd-4075-826d-5f288f155fc7" />
)

### Observations

The original arrangement separates several related activities across the assembly area.

This can result in:

- Additional movement between operations
- Repeated setup of tools and equipment
- Potential waiting for shared resources
- Less direct material flow
- Completed products occupying working areas

The crane is also a shared resource around the wheel-press area, so its availability and movement need to be considered when analyzing the bottleneck.

---

# Proposed Layout

The proposed layout reorganizes the process into dedicated workstations.

(<img width="2048" height="1125" alt="proposed_layout" src="https://github.com/user-attachments/assets/725c07f4-38a1-4acd-91d9-b3aaad6c49b5" />
)

## Proposed Workstation Structure

| Area | Tasks | Purpose |
|---|---|---|
| **Station 1** | Tasks 4–9 | Group the longer sequence of assembly activities |
| **Station 2** | Tasks 10–13 | Continue the assembly sequence |
| **Inspection Station** | Tasks 3 and 19 | Separate inspection from the main assembly workstation |
| **Wheel Press** | Task 14 | Perform the wheel mounting/press operation |
| **Station 3** | Tasks 15–16 | Continue post-mounting activities |
| **Station 4** | Task 17 | Complete the following assembly operation |
| **Completed Wheels** | Task 20 | Temporary area for finished products |

---

## Key Layout Changes

### 1. Create Dedicated Workstations

Related tasks are grouped into specific stations instead of requiring the operator to repeatedly move between different areas.

For example:

**Station 1 → Tasks 4–9**

This allows the required tools and equipment to remain available at that workstation.

### 2. Reduce Repeated Setup

Frequently used tools and equipment can remain at their assigned workstation.

This can reduce repeated setup activity, particularly for **Task 2**.

### 3. Separate Inspection

An independent inspection station allows inspection activities to be handled separately from the main assembly workstation.

This can reduce the possibility of inspection activities blocking the next assembly operation.

### 4. Improve Process Flow

The proposed arrangement creates a more structured sequence:

**Station 1 → Station 2 → Wheel Press → Station 3 → Station 4 → Completed Wheels**

This makes the movement of work easier to follow and reduces unnecessary movement between unrelated areas.

### 5. Add a Completed-Product Area

A dedicated **Completed Wheels** area prevents finished products from occupying the working space of the final workstation.

This allows the workstation to become available for the next unit instead of becoming congested with completed products.

---

# Why This Layout Addresses the Bottleneck

The objective is not to eliminate Step 14 through expensive automation.

Instead, the layout reduces the additional delays surrounding the bottleneck.

The improvement logic is:

**Step 14 identified as bottleneck**

↓

**Automation considered but rejected due to cost and development time**

↓

**Analyze surrounding workflow and layout**

↓

**Group related tasks into dedicated workstations**

↓

**Reduce unnecessary setup, movement, inspection-related blocking, and congestion**

↓

**Improve overall material and work flow**

The proposed layout therefore aims to **reduce the impact of the bottleneck using existing resources**.

---

# Manufacturing Layout Principles Applied

### Minimize Movement

Tools, equipment, and work activities are organized so that workers and materials do not need to travel unnecessarily.

### Balance Workload

Tasks are grouped into stations to create a more structured flow and make bottlenecks easier to identify.

### Improve Material Flow

The layout supports a more logical movement of the product through the assembly process.

### Reduce Waste

The redesign targets forms of Lean waste such as:

- Unnecessary motion
- Transportation
- Waiting
- Excess work-in-process
- Repeated setup

### Improve Visibility

Dedicated workstations make it easier for supervisors and quality teams to monitor individual process steps.

---

# Implementation Considerations

A layout change can itself create temporary disruption, so implementation should be planned carefully.

### Potential Challenges

- Temporary production downtime during relocation
- Limited available space
- Movement of existing equipment
- Worker adjustment to the new workstation structure
- Safety considerations during layout modification
- Possible congestion during the transition

### Mitigation

A practical implementation approach would include:

1. Plan the layout change before physical relocation.
2. Involve operators and relevant engineering/quality teams.
3. Perform changes during planned downtime where possible.
4. Implement the changes in phases if required.
5. Verify safety and material-flow paths before full implementation.
6. Measure cycle time and waiting after implementation.

---

# Expected Benefits

The proposed layout is intended to provide:

- Reduced unnecessary worker movement
- Reduced material transportation
- Lower repeated setup effort
- Less workstation congestion
- Better inspection flow
- Improved visibility of individual processes
- Better utilization of existing resources
- Reduced impact of the wheel-mounting bottleneck
- More consistent production flow

Actual improvements should be validated through **post-implementation time measurements** rather than assumed in advance.

---

# Tools and Concepts Used

- Time Study
- Bottleneck Analysis
- Manufacturing Layout Design
- Process Flow Analysis
- Lean Manufacturing
- Workflow Optimization
- Workstation Design
- Root Cause Thinking
- Continuous Improvement
- Operational Efficiency

---

# Key Learning

The main learning from the simulation was that an industrial engineer does not always need to solve a bottleneck by purchasing new equipment.

A practical solution can come from **better organization of existing resources, improved workflow, and layout redesign**.

The overall approach was:

> **Measure → Identify Bottleneck → Analyze the Process → Consider Constraints → Redesign Layout → Implement → Measure Again**

---

## Interview Explanation

A concise way to explain this project in an interview:

> **“I worked on a Siemens Mobility Operations Industrial Engineer simulation where I analyzed a wheel assembly time study and identified the wheel-mounting operation as the key bottleneck. Initially, automation was considered, but a customized robot was not feasible because of its cost and development time. I therefore worked on a layout-based solution using existing resources. I grouped related tasks into dedicated workstations, separated inspection, and added a completed-product area to reduce unnecessary movement, setup, and congestion. The objective was to improve the overall workflow and reduce the impact of the bottleneck without major new equipment investment.”**

---

## Project Outcome

The project demonstrates the application of **industrial engineering and Lean manufacturing principles** to a practical manufacturing problem, with emphasis on:

**Data-based bottleneck identification → Practical layout redesign → Efficient workflow → Continuous improvement**
