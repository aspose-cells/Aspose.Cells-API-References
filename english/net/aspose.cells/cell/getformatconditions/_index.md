---
title: Cell.GetFormatConditions
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets format conditions which applies to this cell
type: docs
url: /net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Gets format conditions which applies to this cell.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Return Value

Returns [`FormatConditionCollection`](../../formatconditioncollection/) object

### Examples

```csharp
// Called: FormatConditionCollection[] fs = cell.GetFormatConditions();
[Test]
        public void Method_GetFormatConditions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/CellsNet44769.xlsx");
            workbook.Save(Constants.destPath + "CellsNet44769.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet44769.xlsx");
            Cell cell = workbook.Worksheets[1].Cells["B20"];
            FormatConditionCollection[] fs = cell.GetFormatConditions();
           AssertHelper.AreEqual(fs[0][0].Style.Font.Color,Color.Black);
        }
```

### See Also

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


