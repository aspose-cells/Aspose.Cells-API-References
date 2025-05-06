---
title: PivotTable.GetSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Get pivottables source data
type: docs
url: /net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Get pivottable's source data.

```csharp
public string[] GetSource()
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[&amp;quot;Sheet1&amp;quot;].PivotTables[&amp;quot;PivotTable1&amp;quot;].GetSource()[0], &amp;quot;CellsNet44854.xlsx!MyRange&amp;quot;);
[Test]
        public void Method_GetSource()
        {

            var workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet44854.xlsx&quot;);
            Console.WriteLine(&quot;Current data source: {0}&quot;, string.Join(&quot;, &quot;, workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].DataSource));

            workbook.Worksheets[&quot;Sheet1&quot;].Cells[&quot;C2&quot;].PutValue(1000000);
           workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].RefreshData();
           workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].CalculateData();
            Console.WriteLine(&quot;New B20 Value: {0}&quot;, workbook.Worksheets[&quot;Sheet1&quot;].Cells[&quot;B20&quot;].Value);

            workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].ChangeDataSource(new[] { &quot;&apos;&quot; + workbook.FileName + &quot;&apos;!MyRange&quot; }); //workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].ChangeDataSource(new[] { &quot;MyRange&quot; });


            Console.WriteLine(&quot;New data source: {0}&quot;, string.Join(&quot;, &quot;, workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].DataSource));

            workbook.Worksheets[&quot;Sheet1&quot;].Cells[&quot;C2&quot;].PutValue(2000000);
            workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].RefreshData();
           workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].CalculateData();
            Console.WriteLine(&quot;New B20 Value: {0}&quot;, workbook.Worksheets[&quot;Sheet1&quot;].Cells[&quot;B20&quot;].Value);
            Console.WriteLine();
            Assert.AreEqual(workbook.Worksheets[&quot;Sheet1&quot;].PivotTables[&quot;PivotTable1&quot;].GetSource()[0], &quot;CellsNet44854.xlsx!MyRange&quot;);
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet44854.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Get pivottable's source data.

```csharp
public string[] GetSource(bool isOriginal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isOriginal | Boolean | Indicates whether to return original or display data source |

### Examples

```csharp
// Called: string source = pt.GetSource(false)[0];
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET57766.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            string org = pt.GetSource(true)[0];
            Assert.IsTrue(org.StartsWith(@&quot;&apos;\sites\&quot;));
            string source = pt.GetSource(false)[0];
            Assert.IsTrue(source.StartsWith(@&quot;&apos;https:&quot;));
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET57766.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


