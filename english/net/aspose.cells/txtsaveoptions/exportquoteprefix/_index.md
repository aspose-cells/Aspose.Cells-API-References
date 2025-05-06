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
[Test]
        public void Property_ExportQuotePrefix()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(&quot;a\\bcdef\&quot;g&quot;);
            cells[0, 1].PutValue(&quot;f\&quot;g&quot;);
            cells[0, 2].PutValue(&quot;a\\bcdg&quot;);
            cells[0, 3].PutValue(&quot;abcdefg&quot;);
            cells[0, 4].PutValue(&quot;efg&quot;);
            cells[0, 5].PutValue(&quot;&apos;abc&quot;);

            TxtSaveOptions tso = new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
            };

            tso.Separator = &apos;,&apos;;
            CheckOpenSave(wb, tso, &quot;\&quot;a\\bcdef\&quot;\&quot;g\&quot;,\&quot;f\&quot;\&quot;g\&quot;,a\\bcdg,abcdefg,efg,abc\r\n&quot;);
            tso.Separator = &apos;\\&apos;;
            CheckOpenSave(wb, tso, &quot;\&quot;a\\bcdef\&quot;\&quot;g\&quot;\\\&quot;f\&quot;\&quot;g\&quot;\\\&quot;a\\bcdg\&quot;\\abcdefg\\efg\\abc\r\n&quot;);
            tso.SeparatorString = &quot;bcd&quot;;
            CheckOpenSave(wb, tso, &quot;\&quot;a\\bcdef\&quot;\&quot;g\&quot;bcd\&quot;f\&quot;\&quot;g\&quot;bcd\&quot;a\\bcdg\&quot;bcd\&quot;abcdefg\&quot;bcdefgbcdabc\r\n&quot;);
            tso.SeparatorString = &quot;fg&quot;;
            CheckOpenSave(wb, tso, &quot;\&quot;a\\bcdef\&quot;\&quot;g\&quot;fg\&quot;f\&quot;\&quot;g\&quot;fga\\bcdgfg\&quot;abcdefg\&quot;fg\&quot;efg\&quot;fgabc\r\n&quot;);
            tso.ExportQuotePrefix = true; //CELLSJAVA-43396
            CheckOpenSave(wb, tso, &quot;\&quot;a\\bcdef\&quot;\&quot;g\&quot;fg\&quot;f\&quot;\&quot;g\&quot;fga\\bcdgfg\&quot;abcdefg\&quot;fg\&quot;efg\&quot;fg&apos;abc\r\n&quot;);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


