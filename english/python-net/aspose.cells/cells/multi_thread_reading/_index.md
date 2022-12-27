---
title: multi_thread_reading property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1200
url: /python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---

## multi_thread_reading property


Gets or sets whether the cells data model should support Multi-Thread reading.
Default value of this property is false.
### Remarks 


If there are multiple threads to read Row/Cell objects in this collection concurrently,
this property should be set as true, otherwise unexpected result may be produced.
Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection.
Please note, some features cannot support Multi-Thread reading,
such as formatting values(by [Cell.string_value](/cells/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/python-net/aspose.cells/cell#display_string_value), .etc.).
So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

### See Also
* module [aspose.cells](../../)
* class [Cells](/cells/python-net/aspose.cells/cells)
