---
title: on_circular method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---

## on_circular(circular_cells_data) {#collections.abc.Iterator}

Implement this method to do business when calculating formulas with circular references.

### Returns 


Whether the formula engine needs to calculate those cells in circular after this call.
True to let the formula engine continue to do calculation for them.
False to let the formula engine just mark those cells as Calculated.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator | IEnumerator with CalculationCell items representing cells that<br/>depend on circular references. |
### Remarks

In the implementation user may also set the expected value as calculated result
for part/all of those cells so the formula engine will not calculate them recursively.


### See Also
* module [aspose.cells](../../)
* class [AbstractCalculationMonitor](/cells/python-net/aspose.cells/abstractcalculationmonitor)
