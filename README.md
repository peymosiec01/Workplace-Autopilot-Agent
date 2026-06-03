# Workplace Autopilot Agent

## Agent Academy Hackathon 2026 Submission

Workplace Autopilot Agent is a NeuroAI-inspired workplace coordination agent built with Microsoft Copilot Studio, Power Automate, Dataverse, Planner, Teams, and Outlook.

The agent automatically transforms workplace communication into structured, prioritised, and trackable work.

---

# Quick Start

## Import Solution

Import the solution package into your Power Platform environment.

```text
Power Apps
→ Solutions
→ Import Solution
→ WorkplaceAutopilotAgent_1_0_0_1.zip
```

Wait for all components to finish importing.

---

## Configure Connections

Verify the following connections are configured:

* Microsoft Dataverse
* Microsoft Planner
* Microsoft Teams
* Microsoft Outlook
* Power Automate

---

## Publish the Agent

Open:

```text
Workplace Autopilot Agent
```

Publish the agent.

---

# Try the Demo

In MS Teams Channel / Outlook Email, copy and paste the following workplace message and send:

```text
The Friday milestone depends on having the client readiness report ready. This is critical to next steps and the client is expecting an update before Friday.
```

---

## Expected Behaviour

The agent should:

### 1. Extract the Task

Example:

```text
Task:
Prepare Client Readiness Report
```

### 2. Perform NeuroAI Attention Analysis

Example:

```text
Priority Score: 9

Priority Level: High
```

Attention reasons:

```text
- Deadline detected
- Client impact detected
- Dependency detected
```

### 3. Create Goal Memory Record

A Dataverse Goal Memory record is created automatically.

### 4. Create Planner Task

A Planner execution task is created and linked to the memory record.

### 5. Start Tracking

The workplace goal is now being tracked for future follow-up and escalation.

---

# Repository Structure

```text
/
├── solution/
│   └── WorkplaceAutopilotAgent.zip
│
├── screenshots/
│   ├── task-understanding.png
│   ├── neuroai-scoring.png
│   ├── memory-record.png
│   └── planner-task.png
│
├── docs/
│   ├── architecture.png
│   └── demo-script.md
│
└── README.md
```

---

# Solution Components

## Copilot Studio Agent

### Workplace Autopilot Agent

Main orchestration agent responsible for:

* Workplace signal intake
* Tool orchestration
* Autonomous execution

---

## Tool 1

### Task Understanding Tool

Converts workplace communication into structured tasks.

Outputs:

* Task Title
* Task Description
* Due Date
* Category

---

## Tool 2

### NeuroAI Attention Scoring Tool

Applies a NeuroAI-inspired selective attention model.

Evaluates:

* Urgency
* Deadlines
* Dependencies
* Customer impact
* Business context

Outputs:

* Priority Score
* Priority Level
* Attention Reasons
* Cognitive Explanation

---

## Tool 3

### Create Goal Memory Record Tool

Creates a Dataverse memory record representing an unresolved workplace goal.

Stores:

* Workplace signal
* Task details
* Priority information
* Tracking state

This acts as the agent's working memory.

---

## Tool 4

### Planner Task Tool

Creates execution tasks in Microsoft Planner.

Links execution tasks back to memory records.

---

## Monitoring Flows

Included flows:

* Teams Monitor
* Email Monitor
* Teams Intake Monitor
* Email Intake Monitor

These support future autonomous workplace monitoring scenarios.

---

# NeuroAI Architecture

The solution is inspired by cognitive systems and NeuroAI principles.

```text
Workplace Signal
        ↓
Task Understanding
(Perception Layer)
        ↓
NeuroAI Attention Scoring
(Selective Attention Layer)
        ↓
Goal Memory Creation
(Working Memory Layer)
        ↓
Planner Task Creation
(Action Layer)

```

Rather than acting as a traditional chatbot, the agent behaves as a workplace coordinator that understands work, prioritises attention, remembers goals, initiates actions, and supports execution.

---

# Technologies Used

* Microsoft Copilot Studio
* Microsoft Dataverse
* Power Automate
* Microsoft Planner
* Microsoft Teams
* Microsoft Outlook
* Microsoft 365

---

# Author

Moses Babalola

GitHub: @peymosiec01

Agent Academy Hackathon 2026
