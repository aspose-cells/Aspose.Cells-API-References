---
title: Worksheet.DisplayZeros
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. True if zero values are displayed
type: docs
url: /net/aspose.cells/worksheet/displayzeros/
---
## Worksheet.DisplayZeros property

True if zero values are displayed.

```csharp
public bool DisplayZeros { get; set; }
```

### Examples

```csharp
// Called: sheet.DisplayZeros = false;
public void Worksheet_Property_DisplayZeros()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.DisplayZeros = false;
            Cell cell = sheet.Cells[0, 0];
            cell.PutValue(0);
            Style style = cell.GetStyle();
            style.Custom = "0.0;00.00;000.000";
            cell.SetStyle(style);
            Assert.AreEqual("000.000", cell.DisplayStringValue, "DisplayStringValue of Zero for TriCondFormatting");
            Assert.AreEqual("000.000", cell.StringValue, "StringValue of Zero for TriCondFormatting");
            style.Custom = "[>1]0.0;[=0]000.000";
            cell.SetStyle(style);
            Assert.AreEqual("", cell.DisplayStringValue, "DisplayStringValue of Zero for SpecCondFormatting");
            Assert.AreEqual("", cell.StringValue, "StringValue of Zero for SpecCondFormatting");
            style.Custom = "000.000";
            cell.SetStyle(style);
            Assert.AreEqual("", cell.DisplayStringValue, "DisplayStringValue of Zero for SpecCondFormatting");
            Assert.AreEqual("", cell.StringValue, "StringValue of Zero for SpecCondFormatting");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


