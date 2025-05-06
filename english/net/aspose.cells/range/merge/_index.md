---
title: Range.Merge
second_title: Aspose.Cells for .NET API Reference
description: Range method. Combines a range of cells into a single cell
type: docs
url: /net/aspose.cells/range/merge/
---
## Range.Merge method

Combines a range of cells into a single cell.

```csharp
public void Merge()
```

### Remarks

Reference the merged cell via the address of the upper-left cell in the range.

### Examples

```csharp
// Called: sheet.Cells.CreateRange(0, 0, 1, 2).Merge();
[Test]
        public void Method_Merge()
        {
            Workbook wb = new Workbook();
            var sheet = wb.Worksheets[0];
            //create 2x1 merge cell
            sheet.Cells.CreateRange(0, 0, 1, 2).Merge();
            sheet.Cells[0, 0].Value = &quot;&amp;=obj.Property(group:merge)&quot;;
            sheet.Cells[0, 2].Value = &quot;&amp;=obj.AABB&quot;;
            //output template file
            const string templateFile = &quot;template.xlsx&quot;;
            //    wb.Save(templateFile);
            //   Process.Start(&quot;cmd&quot;, $&quot;/c start {templateFile}&quot;);
            var designer = new WorkbookDesigner(wb);
            designer.SetDataSource(&quot;obj&quot;, new[] { new objClass(&quot;Value1&quot;, &quot;Value2&quot;), new objClass(&quot;Value1&quot;, &quot;Value2&quot;), new objClass(&quot;Value1&quot;, &quot;Value3&quot;), new objClass(&quot;Value1&quot;, &quot;Value4&quot;), new objClass(&quot;Value2&quot;, &quot;Value2&quot;) });
            designer.Process();
            CellArea ca = (CellArea)wb.Worksheets[0].Cells.GetMergedAreas()[0];
            Assert.AreEqual(3, ca.EndRow);

            wb.Save(Constants.destPath + &quot;CellsNet52236.xlsx&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


