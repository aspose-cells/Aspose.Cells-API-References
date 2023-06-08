---
title: Cells.FindFormulaContains
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Finds the cell with formula which contains the input string
type: docs
url: /net/aspose.cells/cells/findformulacontains/
---
## Cells.FindFormulaContains method

Finds the cell with formula which contains the input string.

```csharp
[Obsolete("Use Cells.Find(object,Cell,FindOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Cell FindFormulaContains(string formula, Cell previousCell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula to search for. |
| previousCell | Cell | Previous cell with the same formula. This parameter can be set to null if searching from the start. |

### Return Value

Cell object.

### Remarks

Returns null (Nothing) if no cell is found. NOTE: This member is now obsolete. Instead, please use Cells.Find(object,Cell,FindOptions) method with LookInType as LookInType.OnlyFormulas and LookAtType as LookAtType.Contains. This member will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


