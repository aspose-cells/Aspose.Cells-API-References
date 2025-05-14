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
// Called: LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
public void AbstractTextLoadOptions_Property_LoadStyleStrategy()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    Style style = cell.GetStyle();
    style.Pattern = BackgroundType.Solid;
    style.ForegroundColor = Color.Red;
    cell.SetStyle(style);
    StyleFlag flag = new StyleFlag();
    flag.All = true;
    cells.ApplyColumnStyle(1, style, flag);
    cells.ApplyRowStyle(1, style, flag);
    cells.ImportCSV(
        new MemoryStream(Encoding.ASCII.GetBytes("07/14/14,07/14/14\n07/14/14")),
        new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertDateTimeData = true,
                ConvertNumericData = true,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
            },
        0, 0);
    Check43282Style("A1", cell.GetStyle());
    Check43282Style("B1", cells[0, 1].GetStyle());
    Check43282Style("A2", cells[1, 0].GetStyle());
}
```

### See Also

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


