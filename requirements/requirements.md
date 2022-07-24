_This file is generated, do not modify it manually. Use the vimotest-requirements-dsl instead._

## Requirements

**GHERKIN**: Several requirements for the Gherkin-based style of the ViMoTest

**UICOMP**:

**CONTEXT**: Features for the (data) context of ViewModel-based tests

**ASSERT**: Features for the assertion of ViewModel-based tests

**DSL**: Technical Features for the ViMoTest DSL itself

**PL**: Several programming languages shall be supported, to have a flexible approach.

**NONF**: Describes non-functional/quality requirements for the ViMoTest solution


### 1 Gherkin

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **GHERKIN-001** | Support scenarios with Given-When-Then Gherkin syntax | As a test developer, I want to use the familiar Given-When-Then structure of the Gherkin language to write scenarios | Gherkin is well established and provides a suitable style for writing behavior-oriented tests | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Base feature of Gherking, e.g. scenario descriptions with Given-When-Then |
| **GHERKIN-002** | Support BUT-Keyword | As a test developer, I want to use the But-keyword from Gherkin | The but keyword sometimes reads more natural in scenarios | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) |  |
| **GHERKIN-003** | Support data lists | As a test developer, I want to provide list data inputs to describe multiple cases at once |  | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) |  |
| **GHERKIN-004** | Support data tables | As a test developer, I want to provide tabular data inputs to describe multiple cases at once |  | ![NICE TO HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_nicetohave.png) |  |
| **GHERKIN-005** | Support scenario-outlines | As a test developer, I want to provide scenario outlines which gives common context for multiple scenarios | With scenario outlines, test suites might become much simpler when common context is required | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) |  |
### 2 UI Components

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **UICOMP-001** | Support Buttons |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text |
| **UICOMP-002** | Support Check-boxes |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text, Checked-State (tri-state?) |
| **UICOMP-003** | Support Radio Buttons |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text, Selected |
| **UICOMP-004** | Support Labels |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text |
| **UICOMP-005** | Support Image Views |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Image |
| **UICOMP-010** | Support List Views |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, List Items |
| **UICOMP-011** | Support Table Views |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Table Items |
### 3 Context Features

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **CONTEXT-001** | Allow reuse of context (or context parts) |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | E.g. by using the MPS' editor component |
| **CONTEXT-004** | Provide extensible Context Data mechanism (e.g. Hamster Simulator has its own file-based context structure) |  |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | E.g. by using MPS' weaving generator rules |
### 4 Assertion Features

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **ASSERT-001** | Support partial assertions (e.g. 1 Column of a given expected table) | As a test developer, I want to couple my tests only on single aspects | We want that tests fail only for one aspect if possible, (e.g., only for one specific column). But, to allow a good readability of a testcase, sometimes it helps to display more information (e.g. a full table). | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | This is possible since we use a projectional editor |
### 5 Technical DSL Features

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **DSL-001** | ViewModel shall have a built-in "Updating Flag" | As a view-logic developer I want to be able to temporarily disable data-binding updates | For larger or complex UI updates, sometimes data-binding has to be disabled temporarily | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | i.e. to avoid that UIs fire events while larger updates of the ViewModel |
### 6 Programming Languages

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **PL-001** | Support Java | As a Java Developer, I want to generate Java-based ViewModels | Support Java-based UI Frameworks | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | JavaFX in first place |
| **PL-002** | Support C++ | As a C++ Developer, I want to generate C++-based ViewModels | Support C++ based UI Frameworks or native C++ core code | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) |  |
| **PL-003** | Support C# | As a C# Developer, I want to generate C#-based ViewModels | Support C#-based UI Frameworks | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | WPF in first place |
| **PL-004** | Support Typescript | As a Web-Developer I want to generate Typescript-based ViewModels | Support Web-UIs | ![NICE TO HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_nicetohave.png) | More important in future |
### 7 Non-functional/Quality requirements

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **NONF-001** | The ViMoTest DSL shall be easy to learn | As a test developer, I want to quickly learn the ViMoTest DSL | We want that the DSL is easy to use, so that not only MPS-experts can use it | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | Through user studies we will evaluate this |
