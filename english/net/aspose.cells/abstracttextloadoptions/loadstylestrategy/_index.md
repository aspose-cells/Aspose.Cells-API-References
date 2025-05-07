---
title: AbstractTextLoadOptions.LoadStyleStrategy
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Indicates the strategy to apply style for parsed values when converting string value to number or datetime
type: docs
url: /net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Indicates the strategy to apply style for parsed values when converting string value to number or datetime.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Examples

```csharp
// Called: opts.LoadStyleStrategy = TxtLoadStyleStrategy.None;
[Test]
        public void Property_LoadStyleStrategy()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            style.Custom = "yyyy-mm-dd";
            cell.SetStyle(style);
            TxtLoadOptions opts = new TxtLoadOptions();
            opts.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            cells.ImportCSV(new MemoryStream(Encoding.ASCII.GetBytes("2/15/2015")), opts, 0, 0);
            Assert.AreEqual(style.Custom, cell.GetStyle().Custom, "A1.Style.Custom after importing");
            Assert.AreEqual("2015-02-15", cell.StringValue, "A1.StringValue");
        }
```

### See Also

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


