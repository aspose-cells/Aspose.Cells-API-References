---
title: set_metered_key method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/metered/set_metered_key/
is_root: false
---

## set_metered_key(public_key, private_key) {#str-str}

Sets metered public and private key.
If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.



```python
def set_metered_key(self, public_key, private_key):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| public_key | str | public key |
| private_key | str | private key |



### See Also
* module [aspose.cells](../../)
* class [Metered](/cells/python-net/aspose.cells/metered)
