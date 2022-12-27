---
title: start_access_cache method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 280
url: /python-net/aspose.cells/worksheet/start_access_cache/
is_root: false
---

## start_access_cache(opts) {#AccessCacheOptions}

Starts the session that uses caches to access the data in this worksheet.



```python
def start_access_cache(self, opts):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/python-net/aspose.cells/accesscacheoptions) | options of data access |
### Remarks

After finishing the access to the data, [Worksheet.close_access_cache(opts)](/cells/python-net/aspose.cells/worksheet/close_access_cache) should
be invoked with same options to clear all caches and recover normal access mode.


### See Also
* module [aspose.cells](../../)
* class [Worksheet](/cells/python-net/aspose.cells/worksheet)
