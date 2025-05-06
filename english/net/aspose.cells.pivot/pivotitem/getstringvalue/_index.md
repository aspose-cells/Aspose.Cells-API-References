---
title: PivotItem.GetStringValue
second_title: Aspose.Cells for .NET API Reference
description: PivotItem method. Gets the string value of the pivot item If the value is null it will return 
type: docs
url: /net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Gets the string value of the pivot item If the value is null, it will return ""

```csharp
public string GetStringValue()
```

### Examples

```csharp
// Called: if (pitem.GetStringValue().Contains(&amp;quot;长兴县&amp;quot;))
[Test]
        public void Method_GetStringValue()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET52854.xls&quot;);
            PivotTable pt = wb.Worksheets[&quot;Sheet1&quot;].PivotTables[0];
            CellArea rowrang = pt.RowRange;

            int fieldindex = 1;

            Aspose.Cells.Pivot.PivotField pfd = pt.RowFields[fieldindex];

            PivotItemCollection pic = pfd.PivotItems;
            Console.WriteLine(pic.Count);
            Console.WriteLine(pic[0].GetStringValue());
            Console.WriteLine(pic[1].GetStringValue());
            for (int ii = 0; ii &lt; pic.Count; ii++)
            {
                Aspose.Cells.Pivot.PivotItem pitem = pic[ii];
                if (pitem.GetStringValue().Contains(&quot;长兴县&quot;))
                {
                    pitem.IsHidden = true;
                }
                else
                {
                    pitem.IsHidden = false;
                }
            }
            PivotItem item = pt.RowFields[0].PivotItems[0];
            Console.WriteLine(DateTime.Now);
            pt.CalculateData();
            Console.WriteLine(DateTime.Now);
          Assert.AreEqual(&quot;下城区人民检察院&quot;,wb.Worksheets[&quot;Sheet1&quot;].Cells[&quot;B4&quot;].StringValue);
          
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


