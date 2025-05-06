---
title: PivotTable.RefreshData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Refreshes pivottables data and setting from its data source
type: docs
url: /net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Refreshes pivottable's data and setting from it's data source.

```csharp
public PivotRefreshState RefreshData()
```

### Remarks

We will gather data from data source to a pivot cache ,then calculate the data in the cache to the cells. This method is only used to gather all data to a pivot cache.

### Examples

```csharp
// Called: pt.RefreshData();
[Test]
        public void Method_RefreshData()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET44549_&quot;;
            Workbook wb = new Workbook(filePath + &quot;source.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[0];
            foreach (PivotTable pt in sheet.PivotTables)
            {
                pt.RefreshData();
                pt.CalculateData();
            }
            wb.Save(Constants.PivotTableDestPath + &quot;NET44549.xlsx&quot;);
            Assert.AreEqual(sheet.Cells[&quot;G8&quot;].StringValue, &quot;6&quot;);
            Assert.AreEqual(sheet.Cells[&quot;G9&quot;].StringValue, &quot;12&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET44549.pdf&quot;);

            wb = new Workbook(filePath + &quot;sample.xlsx&quot;);
            sheet = wb.Worksheets[0];
            foreach (PivotTable pt in sheet.PivotTables)
            {
                pt.RefreshData();
                pt.CalculateData();
            }
            Assert.AreEqual(sheet.Cells[&quot;B8&quot;].StringValue, &quot;10&quot;);
            Assert.AreEqual(sheet.Cells[&quot;C8&quot;].StringValue, &quot;22&quot;);
            Assert.AreEqual(sheet.Cells[&quot;D8&quot;].StringValue, &quot;32&quot;);
            Assert.AreEqual(sheet.Cells[&quot;E8&quot;].StringValue, &quot;3.2&quot;);
            Assert.AreEqual(sheet.Cells[&quot;F8&quot;].StringValue, &quot;3.2&quot;);
            Assert.AreEqual(sheet.Cells[&quot;G8&quot;].StringValue, &quot;70.4&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;NET44549sample_out.pdf&quot;);
        }
```

### See Also

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Refreshes pivottable's data and setting from it's data source with options.

```csharp
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The options for refreshing data source of pivot table. |

### Examples

```csharp
// Called: pivotTable.RefreshData(refreshOption);
public static void Method_PivotTableRefreshOption_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[0, 1].Value = &quot;Year&quot;;
            worksheet.Cells[0, 2].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;=Sheet1!A1:C5&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Create an instance of PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Refresh the pivot table with the specified options
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save(&quot;PivotTableRefreshOptionExample.xlsx&quot;);
        }
```

### See Also

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


