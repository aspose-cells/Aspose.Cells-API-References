---
title: FormatConditionCollection.GetCellArea
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Gets the conditional formatted cell range by index
type: docs
url: /net/aspose.cells/formatconditioncollection/getcellarea/
---
## FormatConditionCollection.GetCellArea method

Gets the conditional formatted cell range by index.

```csharp
public CellArea GetCellArea(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the conditional formatted cell range. |

### Return Value

the conditional formatted cell range

### Examples

```csharp
// Called: CellArea ca = fcs.GetCellArea(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET55185.xlsx");
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = Aspose.Cells.Ods.OpenDocumentFormatVersionType.Odf13;
            workbook.Save(Constants.destPath + "CELLSNET55185.ods", saveOptions);
            workbook = new Workbook(Constants.destPath + "CELLSNET55185.ods");
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            CellArea ca = fcs.GetCellArea(0);
            Assert.AreEqual(ca.EndRow, 0xFFFFF);
            Assert.AreEqual(2, ca.StartColumn);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


