---
title: ListColumn.Formula
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the formula of the list column
type: docs
url: /net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Gets and sets the formula of the list column.

```csharp
public string Formula { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;=Table2[[#Headers],[Discount]]&amp;quot;, lo.Formula);
[Test]
        public void Property_Formula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET52840.xlsx&quot;);
            Worksheet src = workbook.Worksheets[0];
            var srcRange = src.Cells.CreateRange(&quot;A1:F3&quot;);
           
            int index = workbook.Worksheets.Add();
            Worksheet dst = workbook.Worksheets[index];
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange(&quot;A1:F3&quot;);
            ;

            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;
            dstRange.Copy(srcRange, pasteOptions);
            ListObject table = workbook.Worksheets[1].ListObjects[0];
           ListColumn lo = table.ListColumns[table.ListColumns.Count - 1];
            Assert.AreEqual(&quot;=Table2[[#Headers],[Discount]]&quot;, lo.Formula);
            //CELLSNET-52834
            Assert.AreEqual(&quot;=Table2[[#Headers],[Discount]]&quot;, dst.Cells[&quot;F2&quot;].Formula);
            workbook.Save(Constants.destPath + &quot;CELLSNET52840.xlsx&quot;);
        }
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


