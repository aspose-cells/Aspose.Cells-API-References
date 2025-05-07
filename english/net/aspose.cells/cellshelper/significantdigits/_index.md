---
title: CellsHelper.SignificantDigits
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper property. Gets and sets the number of significant digits. The default value is 17
type: docs
url: /net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Gets and sets the number of significant digits. The default value is 17.

```csharp
public static int SignificantDigits { get; set; }
```

### Remarks

Only could be 15 or 17 now.

### Examples

```csharp
// Called: CellsHelper.SignificantDigits = 15;
[Test]
        public void Property_SignificantDigits()
        {
            CellsHelper.SignificantDigits = 15;
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].Value = 101956.70469425319;

            workbook.Save(Constants.destPath + "CELLSNET44986.xlsx");
            CellsHelper.SignificantDigits = 17;
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


