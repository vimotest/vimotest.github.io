_This file is generated, do not modify it manually. Use the vimotest-requirements-dsl instead._

## Requirements

**GHERKIN**: Several requirements for the Gherkin-based style of the ViMoTest

**UICOMP**: The ViMoTest DSL shall provide several common UI components like buttons, check-boxes, tables etc.

**CONTEXT**: Features for the (data) context of ViewModel-based tests

**ASSERT**: Features for the assertion of ViewModel-based tests

**DSL**: Technical Features for the ViMoTest DSL itself

**CHECK**: Static checks for ViMoTest models

**PL**: Several programming languages shall be supported, to have a flexible approach.

**GEN**: Requirements related to the generation and extensibility of the MPS-based DSL

**NONF**: Describes non-functional/quality requirements for the ViMoTest solution


### 1 Gherkin

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **GHERKIN-001** | Support scenarios with Given-When-Then Gherkin syntax | As a test developer, I want to use the familiar Given-When-Then structure of the Gherkin language to write scenarios | Gherkin is well established and provides a suitable style for writing behavior-oriented tests | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Base feature of Gherking, e.g. scenario descriptions with Given-When-Then |
| **GHERKIN-002** | Integrated BDD | As a test developer, I want to mix the Given-When-Then parts directly with the test case elements | The but keyword sometimes reads more natural in scenarios | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | E.g. <br/>GIVEN <some-xml>...</> data<br/>WHEN LoadView() is called<br/>THEN assert <BUTTON> is enabled |
| **GHERKIN-003** | Support BUT-Keyword | As a test developer, I want to use the But-keyword from Gherkin | The but keyword sometimes reads more natural in scenarios | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) |  |
| **GHERKIN-004** | Support scenario-outlines | As a test developer, I want to provide scenario outlines which gives common context for multiple scenarios | With scenario outlines, test suites might become much simpler when common context is required | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) |  |
| **GHERKIN-010** | Support data lists | As a test developer, I want to provide list data inputs to describe multiple cases at once |  | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) |  |
| **GHERKIN-011** | Support data tables | As a test developer, I want to provide tabular data inputs to describe multiple cases at once |  | ![NICE TO HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_nicetohave.png) |  |

### 2 UI Components

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **UICOMP-001** | Support Buttons | As a view developer, I need to support buttons | Buttons are needed in mostly any UI | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text |
| **UICOMP-002** | Support Check-boxes | As a view developer, I need to support check-boxes |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text, Checked-State (tri-state?) |
| **UICOMP-003** | Support Radio Buttons | As a view developer, I need to support radio buttons |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text, Selected |
| **UICOMP-004** | Support Labels | As a view developer, I need to support labels |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Text |
| **UICOMP-005** | Support Image Views | As a view developer, I need to support icons/images |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Image |
| **UICOMP-006** | Support Combo-boxes | As a view developer, I need to support comboboxes |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Selected Text, Text Values |
| **UICOMP-010** | Support List Views | As a view developer, I need to support list views |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, List Items |
| **UICOMP-011** | Support Table Views | As a view developer, I need to support table views |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, Table Items |
| **UICOMP-012** | Support Tree Views | As a view developer, I need to support tree views |  | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Properties: Visibility, Enabled, hierarchical TreeView Items |
| **UICOMP-020** | Horizontal Layout | As a view developer, I want to have a visual layout container to visualize view components horizontally next to each other | better visualize intended layout | ![NICE TO HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_nicetohave.png) | e.g. for a button bar |
| **UICOMP-050** | Custom Component Fields | As a view developer, I want to be able to define (unsupported) custom fields for any UI component, including nested elements like TableRows | flexibility | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | e.g. for an additional boolean in a table row, if it's text shall be highlighted in bold |
| **UICOMP-051** | Color Literal Support | As a view developer, I want to be able to have support for coloring by color codes/literals of text-based components |  | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | specific foreground, background, selection colors |
| **UICOMP-052** | Color Symbol Support | As a view developer, I want to be able to have support for logical coloring enumerations for text-based components |  | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | specific foreground, background, selection colors |

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
| **DSL-002** | Provide Command abstraction for view inputs | As a view-logic developer, I want to add UI commands and bind them with UI frameworks directly | WPF provides UI commands, with an Execute() and a CanExecute() method. Command-bindings simplify the usage of such view inputs | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | Examples: WPF Command Bindings |
| **DSL-003** | Provide virtual (domain-oriented) properties for ViewModel fields | As a view-logic developer, I want to have the possibility to define more UI-component independent properties, which are the source for UI-component-specific properties | Many people implement MVVM explicitly without naming/orienting ViewModel-fields "UI-component-specific", but more domain-oriented. E.g. a textbox's text-property for a person-name can be named "personName" (domain-oriented) or "personNameTextBoxText" (UI-component-specific). The latter is more like ViMoTest shall be designed, while the former one is more the "virtual source" for it. Also, often one "virtual property" might be the source for multiple "UI-component-specific" fields. | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Important to be aligned to the MVVM practice which is often done |

### 6 Static Checks

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **CHECK-001** | Check Naming Conventions | As a view/test developer, I want to specify consistent names |  | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | e.g. consistently set "Btn" suffix/prefix or not |

### 7 Programming Languages

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **PL-001** | Support Java | As a Java Developer, I want to generate Java-based ViewModels | Support Java-based UI Frameworks | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | JavaFX in first place |
| **PL-002** | Support C++ | As a C++ Developer, I want to generate C++-based ViewModels | Support C++ based UI Frameworks or native C++ core code | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) |  |
| **PL-003** | Support C# | As a C# Developer, I want to generate C#-based ViewModels | Support C#-based UI Frameworks | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | WPF in first place |
| **PL-004** | Support Typescript | As a Web-Developer I want to generate Typescript-based ViewModels | Support Web-UIs | ![NICE TO HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_nicetohave.png) | More important in future |

### 8 Generation

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **GEN-001** | Replacable viewmodel field in test suites | As a language programmer, I want to build custom test suite DSL extensions with flexible viewmodel fields | The viewmodel field in a Test suite shall be replacable, e.g. for a DSL extension which defines a special Test-Suite baseclass | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Used for hamster simulator |
| **GEN-002** | Controllable output names | As a test developer, I want to have optional control over generated class/field/package names | For interoperability to existing solutions, the ViMoTest approach can be build up-on existing classes | ![MUST HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_musthave.png) | Necessary for using existing hamster simulator |

### 9 Non-functional/Quality requirements

| ID | Requirement | User Story | Reason | Importance | Notes |
|----|-------------|------------|--------|------------|-------|
| **NONF-001** | The ViMoTest DSL shall be easy to learn | As a test developer, I want to quickly learn the ViMoTest DSL | We want that the DSL is easy to use, so that not only MPS-experts can use it | ![SHOULD HAVE](https://github.com/vimotest/vimotest.github.io/raw/main/images//req_importance_shouldhave.png) | Through user studies we will evaluate this |

