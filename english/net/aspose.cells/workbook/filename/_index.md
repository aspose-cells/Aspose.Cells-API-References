---
title: Workbook.FileName
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the current file name
type: docs
url: /net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Gets and sets the current file name.

```csharp
public string FileName { get; set; }
```

### Remarks

If the file is opened by stream and there are some external formula references, please set the file name.

### Examples

```csharp
// Called: workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "'" + workbook.FileName + "'" + "!MyRange" });
[Test]
        public void Property_FileName()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET44854_";

            Console.WriteLine(filePath + "PivotTableNamedRangeDataSoruce.xlsx");
            var workbook = new Workbook(filePath + "PivotTableNamedRangeDataSoruce.xlsx");
            Console.WriteLine("Current data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(1000000);
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);

            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "'" + workbook.FileName + "'" + "!MyRange" });
            //workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "MyRange" }); 


            Console.WriteLine("New data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(2000000);
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);
            Console.WriteLine();

            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + "NET44854.xlsx");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


