﻿---
title: Aspose::Cells::NameCollection::RemoveAt method
linktitle: RemoveAt
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::NameCollection::RemoveAt method. Remove the name at the specific index in C++.'
type: docs
weight: 1000
url: /cpp/aspose.cells/namecollection/removeat/
---
## NameCollection::RemoveAt method


Remove the name at the specific index.

```cpp
void Aspose::Cells::NameCollection::RemoveAt(int32_t index)
```


| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | index of the [Name](../../name/) to be removed. |
## Remarks



Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better. 
## See Also

* Class [Vector](../../vector/)
* Class [NameCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
