---
title: PivotTable.Indent
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form
type: docs
url: /net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

Specifies the indentation increment for compact axis and can be used to set the Report Layout to Compact Form.

```csharp
public int Indent { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(5, w.Worksheets[1].PivotTables[0].Indent);
[Test]
        public void Property_Indent()
        {
            Workbook w = new Workbook(Constants.PivotTableSourcePath + &quot;CellsJava46061_1.xlsx&quot;);
            Assert.AreEqual(5, w.Worksheets[1].PivotTables[0].Indent);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


