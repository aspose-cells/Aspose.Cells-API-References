---
title: NameCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Remove the name at the specific index
type: docs
url: /net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Remove the name at the specific index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | index of the Name to be removed. |

### Remarks

Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better.

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


