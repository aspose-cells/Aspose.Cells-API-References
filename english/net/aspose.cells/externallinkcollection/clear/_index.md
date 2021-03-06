---
title: Clear
second_title: Aspose.Cells for .NET API Reference
description: Removes all external links.
type: docs
weight: 40
url: /net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Removes all external links.

```csharp
public void Clear()
```

### Remarks

When removing external links, all formulas that reference to them will be removed too because the references become invalid.

### See Also

* class [ExternalLinkCollection](../../externallinkcollection)
* namespace [Aspose.Cells](../../externallinkcollection)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Removes all external links.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Whether update all references of external links as references of current workbook itself. |

### Remarks

If references are required to be updated, references to external links in formulas will be changed to current workbook. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()". If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.

### See Also

* class [ExternalLinkCollection](../../externallinkcollection)
* namespace [Aspose.Cells](../../externallinkcollection)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
