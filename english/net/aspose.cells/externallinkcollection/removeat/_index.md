---
title: ExternalLinkCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection method. Removes the specified external link from the workbook
type: docs
url: /net/aspose.cells/externallinkcollection/removeat/
---
## RemoveAt(int) {#removeat}

Removes the specified external link from the workbook.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the external link to be removed. |

### Remarks

When removing the external link, all formulas that reference to it will be removed too because the references become invalid.

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_1}

Removes the specified external link from the workbook.

```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the external link to be removed. |
| updateReferencesAsLocal | Boolean | Whether update all references of given external link to reference of current workbook itself. Check  to get more details about this parameter. |

### See Also

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


