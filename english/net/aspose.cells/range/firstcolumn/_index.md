---
title: Range.FirstColumn
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the index of the first column of the range
type: docs
url: /net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

Gets the index of the first column of the range.

```csharp
public int FirstColumn { get; }
```

### Examples

```csharp
// Called: var cloneRange = insertRange.Worksheet.Cells.CreateRange(insertIndex + sourceRange.FirstRow, sourceRange.FirstColumn, sourceRange.RowCount, sourceRange.ColumnCount);
[Test]
        public void Property_FirstColumn()
        {
            Stopwatch watch = new Stopwatch();
            watch.Start();
            //const int Iterations = 10000; // slow but ok
            const int Iterations = 50000; // v. slow

            var template = new Aspose.Cells.Workbook();
            var templateWorksheet = template.Worksheets[0];
            var range = templateWorksheet.Cells.CreateRange(&quot;A1&quot;, &quot;A1&quot;);
            range.Name = &quot;One&quot;;
            range = templateWorksheet.Cells.CreateRange(&quot;B1&quot;, &quot;B1&quot;);
            range.Name = &quot;Two&quot;;
            range = templateWorksheet.Cells.CreateRange(&quot;A1&quot;, &quot;B1&quot;);
            range.Name = &quot;Insert&quot;;

            var work = new Aspose.Cells.Workbook();
            var insertRang = work.Worksheets[0].Cells.CreateRange(&quot;A1&quot;, &quot;B1&quot;);
            insertRang.Name = &quot;Insert&quot;;
            var insertRange = work.Worksheets.GetRangeByName(&quot;Insert&quot;);
            int insertIndex = insertRange.FirstRow + insertRange.RowCount;
            insertRange.Worksheet.Cells.InsertRows(insertIndex, 1 + Iterations, true);
            // Copy ranges
            var ranges = templateWorksheet.Workbook.Worksheets.GetNamedRanges();
            for (int i = 0; i &lt; Iterations; i++, insertIndex++)
            {

                insertRange.Worksheet.Cells.CopyRows(templateWorksheet.Cells, 0, insertIndex, 1);


                foreach (var sourceRange in ranges)
                {
                    var cloneRange = insertRange.Worksheet.Cells.CreateRange(insertIndex + sourceRange.FirstRow, sourceRange.FirstColumn, sourceRange.RowCount, sourceRange.ColumnCount);
                    cloneRange.Name = sourceRange.Name;
                }
                // Set a value. This must set a dirty flag as without it the name removes are fast
                work.Worksheets.GetRangeByName(&quot;One&quot;)[0, 0].PutValue(&quot;123&quot;, true);
                work.Worksheets.Names.Remove(&quot;One&quot;);
                work.Worksheets.Names.Remove(&quot;Two&quot;);
            }
            Assert.AreEqual(1, work.Worksheets.ExternalLinks.Count);
            watch.Stop();
            int timeLimit = 10;
            Assert.IsTrue(watch.Elapsed.TotalSeconds &lt; timeLimit, 
                string.Format(&quot;The time cost exceeded the limited [{0}] seconds.&quot;, timeLimit));
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


