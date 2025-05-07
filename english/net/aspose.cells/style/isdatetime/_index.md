---
title: Style.IsDateTime
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates whether the number format is a date format
type: docs
url: /net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Indicates whether the number format is a date format.

```csharp
public bool IsDateTime { get; }
```

### Examples

```csharp
// Called: if (!style.IsDateTime)
[Test]
        public void Property_IsDateTime()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            style.Custom = "[mm]";
            if (!style.IsDateTime)
            {
                Assert.Fail("Style.IsDateTime should be true for [mm]");
            }

            style.Custom = "#.##0\" \";[Magenta]-#.##0\" \"";
            if (style.IsDateTime)
            {
                Assert.Fail("Style.IsDateTime should be false for [Magenta]");
            }
            cell.SetStyle(style);
            cell.PutValue(-12.3456);
            Style s = cell.GetDisplayStyle();
            AssertHelper.AreEqual(Color.Magenta, s.Font.Color, "DisplayStyle.Font.Color");
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


