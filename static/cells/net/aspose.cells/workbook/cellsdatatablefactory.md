##Workbook.CellsDataTableFactory
Workbook property. Gets the factory for building ICellsDataTable from custom objects
## Workbook.CellsDataTableFactory property
Gets the factory for building ICellsDataTable from custom objects
```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomData
{
public int Id { get; set; }
public string Name { get; set; }
public int Age { get; set; }
}
public class WorkbookPropertyCellsDataTableFactoryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
List<CustomData> dataList = new List<CustomData>
{
new CustomData { Id = 1, Name = "John Doe", Age = 30 },
new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
};
// Get CellsDataTableFactory from workbook property
CellsDataTableFactory factory = workbook.CellsDataTableFactory;
// Create data table from list
ICellsDataTable dataTable = factory.GetInstance(dataList);
// Import data to worksheet
sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());
// Save outputs
workbook.Save("CellsDataTableFactoryDemo.xlsx");
}
}
}
```
### See Also
* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
