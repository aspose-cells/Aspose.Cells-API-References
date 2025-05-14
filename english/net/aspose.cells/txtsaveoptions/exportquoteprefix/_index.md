---
title: TxtSaveOptions.ExportQuotePrefix
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Indicates whether the single quote sign should be exported as part of the value of one cell when QuotePrefix is true for it. Default is false
type: docs
url: /net/aspose.cells/txtsaveoptions/exportquoteprefix/
---
## TxtSaveOptions.ExportQuotePrefix property

Indicates whether the single quote sign should be exported as part of the value of one cell when [`QuotePrefix`](../../style/quoteprefix/) is true for it. Default is false.

```csharp
public bool ExportQuotePrefix { get; set; }
```

### Examples

```csharp
// Called: tso.ExportQuotePrefix = true; //CELLSJAVA-43396
public void TxtSaveOptions_Property_ExportQuotePrefix()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[0, 0].PutValue("a\\bcdef\"g");
    cells[0, 1].PutValue("f\"g");
    cells[0, 2].PutValue("a\\bcdg");
    cells[0, 3].PutValue("abcdefg");
    cells[0, 4].PutValue("efg");
    cells[0, 5].PutValue("'abc");

    TxtSaveOptions tso = new TxtSaveOptions()
    {
        Encoding = Encoding.ASCII,
    };

    tso.Separator = ',';
    CheckOpenSave(wb, tso, "\"a\\bcdef\"\"g\",\"f\"\"g\",a\\bcdg,abcdefg,efg,abc\r\n");
    tso.Separator = '\\';
    CheckOpenSave(wb, tso, "\"a\\bcdef\"\"g\"\\\"f\"\"g\"\\\"a\\bcdg\"\\abcdefg\\efg\\abc\r\n");
    tso.SeparatorString = "bcd";
    CheckOpenSave(wb, tso, "\"a\\bcdef\"\"g\"bcd\"f\"\"g\"bcd\"a\\bcdg\"bcd\"abcdefg\"bcdefgbcdabc\r\n");
    tso.SeparatorString = "fg";
    CheckOpenSave(wb, tso, "\"a\\bcdef\"\"g\"fg\"f\"\"g\"fga\\bcdgfg\"abcdefg\"fg\"efg\"fgabc\r\n");
    tso.ExportQuotePrefix = true; //CELLSJAVA-43396
    CheckOpenSave(wb, tso, "\"a\\bcdef\"\"g\"fg\"f\"\"g\"fga\\bcdgfg\"abcdefg\"fg\"efg\"fg'abc\r\n");
}
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


