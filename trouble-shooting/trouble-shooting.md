# Troubleshooting

**Weird errors, e.g. Hamster framework classes not found when executing 'makeAndTestHamsterSimulatorViewTest'**

This was caused in the past by executing the MPS' `Optimize Imports` and `Fix Module Imports`.
Be extremely careful with this features, since they might remove dependencies which are indeed required.
If using them: Always do it in a separate commit.
