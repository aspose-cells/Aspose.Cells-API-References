---
title: PivotTable.DataSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the data source of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/datasource/
---
## PivotTable.DataSource property

Gets and sets the data source of the pivot table.

```csharp
public string[] DataSource { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Current data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));
private void Property_DataSource(string fileName, string outName)
        {
            Console.WriteLine(fileName);
            var workbook = new Workbook(fileName);
            Console.WriteLine("Current data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(1000000);
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshDataOnOpeningFile = true;
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);

            //workbook.Worksheets.Names["MyRange"].RefersTo

            //workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { workbook.Worksheets.Names["MyRange"].RefersTo });
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "MyRange" });

            Console.WriteLine("New data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(2000000);
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshDataOnOpeningFile = true;
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);
            Console.WriteLine();

            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + outName);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


