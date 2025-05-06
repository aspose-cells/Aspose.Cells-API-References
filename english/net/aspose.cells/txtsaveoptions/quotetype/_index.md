---
title: TxtSaveOptions.QuoteType
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Gets or sets how to quote values in the exported text file
type: docs
url: /net/aspose.cells/txtsaveoptions/quotetype/
---
## TxtSaveOptions.QuoteType property

Gets or sets how to quote values in the exported text file.

```csharp
public TxtValueQuoteType QuoteType { get; set; }
```

### Examples

```csharp
// Called: QuoteType = TxtValueQuoteType.Always});
[Test]
        public void Property_QuoteType()
        {
            int[][] cols = new int[][]
            {
                null, null,
                new int[]{2, 4},
                new int[]{4, 5},
                null,
                new int[]{4, 6}, 
            };
            object[][] vals = new object[][]
            {
                null, null,
                new object[]{&quot;C3&quot;, 1},
                new object[]{&quot;E4&quot;, true},
                null,
                new object[]{&quot;#VALUE!&quot;, 2.5},
            };
            MemoryStream s = new MemoryStream(1024);
            Workbook wbS = CreateForTestTrim(cols, vals);

            wbS.Save(s, new TxtSaveOptions(){Encoding = Encoding.ASCII, TrimLeadingBlankRowAndColumn = false});
            s.Seek(0, SeekOrigin.Begin);
            TextReader r = new StreamReader(s, Encoding.ASCII);
            if (r.ReadLine() != &quot;&quot;)
            {
                Assert.Fail(&quot;First line of the saved csv should be empty. Content of the saved csv file:\n&quot;
                    + Encoding.ASCII.GetString(s.ToArray()));
            }
            s.Seek(0, SeekOrigin.Begin);
            Workbook wbD = new Workbook(s, new TxtLoadOptions(){Encoding = Encoding.ASCII});
            CheckForTestTrim(wbD.Worksheets[0].Cells, 0, 0, cols, vals);

            s.Seek(0, SeekOrigin.Begin);
            wbS.Save(s, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                TrimLeadingBlankRowAndColumn = false,
                KeepSeparatorsForBlankRow = true });
            s.Seek(0, SeekOrigin.Begin);
            r = new StreamReader(s, Encoding.ASCII);
            if (r.ReadLine() != &quot;,,,,,,&quot;)
            {
                Assert.Fail(&quot;First line of the saved csv should be \&quot;,,,,,,\&quot;. Content of the saved csv file:\n&quot;
                    + Encoding.ASCII.GetString(s.ToArray()));
            }
            s.Seek(0, SeekOrigin.Begin);
            wbD = new Workbook(s, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            CheckForTestTrim(wbD.Worksheets[0].Cells, 0, 0, cols, vals);

            s.Seek(0, SeekOrigin.Begin);
            wbS.Save(s, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                TrimLeadingBlankRowAndColumn = false,
                KeepSeparatorsForBlankRow = true,
                QuoteType = TxtValueQuoteType.Always});
            s.Seek(0, SeekOrigin.Begin);
            r = new StreamReader(s, Encoding.ASCII);
            if (r.ReadLine() != &quot;\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;&quot;)
            {
                Assert.Fail(&quot;First line of the saved csv should be \&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;,\&quot;\&quot;. Content of the saved csv file:\n&quot;
                    + Encoding.ASCII.GetString(s.ToArray()));
            }
            s.Seek(0, SeekOrigin.Begin);
            wbD = new Workbook(s, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            CheckForTestTrim(wbD.Worksheets[0].Cells, 0, 0, cols, vals);
        }
```

### See Also

* enum [TxtValueQuoteType](../../txtvaluequotetype/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


