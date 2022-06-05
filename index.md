# ViMoTest Prototype - A MPS based prototype for the ViewModel-based Testing approach

In this repository, you can find a prototype where the ViewModel-based Testing (ViMoTest) approach is basically demonstrated.
It is based on the language workbench JetBrains MPS, which supports the approach with its projectional editors and powerful language modularity features.

## What is ViewModel-based Testing?

ViewModel-based Testing is meant to be an automated testing approach, where (unit) tests are written against a specific abstraction layer, i.e. ViewModels.
ViewModels are an architectural pattern, mainly known from the Microsoft's MVVM (Model-View-ViewModel) pattern.

This approach tries to tackle the problem of fragility in UI-based tests.
By using ViewModels, a large portion of the View-Logic (presenter, controller code) can be written isolated from concrete UI frameworks, and enables a good testability.
