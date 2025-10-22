##DataModel.Tables
DataModel property. Gets all tables in the data model
## DataModel.Tables property
Gets all tables in the data model.
```csharp
public DataModelTableCollection Tables { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;
namespace AsposeCellsExamples
{
public class DataModelPropertyTablesDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Access the data model
DataModel dataModel = wb.DataModel;
// Get tables collection and show count
Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
// Load sample workbook with data model
string sourceFile = "example.xlsb";
if (System.IO.File.Exists(sourceFile))
{
Workbook sampleWorkbook = new Workbook(sourceFile);
DataModel sampleDataModel = sampleWorkbook.DataModel;
// Access tables collection
DataModelTableCollection tables = sampleDataModel.Tables;
Console.WriteLine($"Tables count in sample file: {tables.Count}");
// Iterate through tables
foreach (DataModelTable table in tables)
{
Console.WriteLine($"Table name: {table.Name}");
}
}
else
{
Console.WriteLine($"Sample file '{sourceFile}' not found. Create an Excel file with data model to see tables information.");
}
}
}
}
```
### See Also
* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)
