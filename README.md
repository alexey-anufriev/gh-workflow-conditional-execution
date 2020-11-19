## `workflow_dispatch` inputs and conditional execution

Conditional execution of workflow steps triggered with `workflow_dispatch` event based on provided inputs.

Input definition:
```
workflow_dispatch:
  inputs:
    test:
      default: 'y'
```

Condition:
```
if: github.event.inputs.test == 'y'
```

## PR name as condition for workfllow steps execution
