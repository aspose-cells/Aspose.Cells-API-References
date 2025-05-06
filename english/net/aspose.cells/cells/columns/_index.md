---
title: Cells.Columns
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Column objects that represents the individual columns in this worksheet
type: docs
url: /net/aspose.cells/cells/columns/
---
## Cells.Columns property

Gets the collection of [`Column`](../../column/) objects that represents the individual columns in this worksheet.

```csharp
public ColumnCollection Columns { get; }
```

### Examples

```csharp
// Called: cells.Columns[0].ApplyStyle(s, sf);
[Test]
        public void Property_Columns()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Style s = wb.CreateStyle();
            s.Custom = &quot;0.00E+0&quot;;
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(s, sf);
            Cell cell = cells[0, 0];
            cell.PutValue(12345);
            cell.SetStyle(wb.DefaultStyle);
            Assert.AreEqual(&quot;12345\r\n&quot;,
                SaveAsCsv(wb, new TxtSaveOptions()
                {
                    Encoding = Encoding.ASCII,
                }));
        }
```

### See Also

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


