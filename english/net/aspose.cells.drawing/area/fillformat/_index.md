---
title: Area.FillFormat
second_title: Aspose.Cells for .NET API Reference
description: Area property. Represents a FillFormat object that contains fill formatting properties for the specified chart or shape
type: docs
url: /net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Represents a `FillFormat` object that contains fill formatting properties for the specified chart or shape.

```csharp
public FillFormat FillFormat { get; }
```

### Examples

```csharp
// Called: aseries.Area.FillFormat.Pattern = FillPattern.Gray10;
[Test]
        public void Property_FillFormat()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Series aseries = chart.NSeries[0];
            aseries.Area.FillFormat.Pattern = FillPattern.Gray10;

            checkFillPattern_Gray10(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkFillPattern_Gray10(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkFillPattern_Gray10(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


