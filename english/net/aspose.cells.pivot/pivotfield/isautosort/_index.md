---
title: PivotField.IsAutoSort
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is automatically sorted
type: docs
url: /net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Indicates whether the specified PivotTable field is automatically sorted.

```csharp
public bool IsAutoSort { get; set; }
```

### Examples

```csharp
// Called: p.RowFields[0].IsAutoSort = true;
[Test]
        public void Property_IsAutoSort()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET44237_&quot;;

            var wbk = new Workbook();
            var wks = wbk.Worksheets[0];
            wks.Cells[0, 0].PutValue(&quot;Col1&quot;);
            wks.Cells[0, 1].PutValue(&quot;Col2&quot;);
            for (int row = 1; row &lt;= 10; row++)
            {
                wks.Cells[row, 0].PutValue(row / 2 == 0 ? &quot;A&quot; : &quot;B&quot;);
                wks.Cells[row, 1].PutValue(5 + row / 2);
            }

            var index = wks.PivotTables.Add(&quot;A1:B11&quot;, &quot;I1&quot;, &quot;MyTable&quot;);
            var p = wks.PivotTables[index];
            p.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Col1&quot;);
            index = p.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;Col2&quot;);
            var f = p.DataFields[index];
            f.Function = ConsolidationFunction.Count;


            p.RowFields[0].IsAutoSort = true;
            //Setting the field auto show ascend. 
            p.RowFields[0].IsAscendSort = false;

            //Setting the auto show using field(data field). 
            p.RowFields[0].AutoShowField = 0;

            p.RefreshData();
            p.CalculateData();

            Assert.AreEqual(wks.Cells[&quot;J2&quot;].StringValue, &quot;9&quot;);
            //wbk.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


