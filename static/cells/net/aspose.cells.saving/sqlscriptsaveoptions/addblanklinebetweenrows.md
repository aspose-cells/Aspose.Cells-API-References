##SqlScriptSaveOptions.AddBlankLineBetweenRows
SqlScriptSaveOptions property. Insert blank line between each data
## SqlScriptSaveOptions.AddBlankLineBetweenRows property
Insert blank line between each data.
```csharp
public bool AddBlankLineBetweenRows { get; set; }
```
### Remarks
If [`Separator`](../separator/) is '\n' , it's better to set this property as true to increase readability.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;
namespace AsposeCellsExamples
{
public class SqlScriptSaveOptionsPropertyAddBlankLineBetweenRowsDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue("Jane");
// Configure SQL save options
SqlScriptSaveOptions options = new SqlScriptSaveOptions
{
OperatorType = SqlScriptOperatorType.Insert,
TableName = "Employees",
IdName = "ID",
AddBlankLineBetweenRows = true,
CreateTable = true
};
// Save to memory stream and get SQL script as string
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, options);
stream.Position = 0;
using (StreamReader reader = new StreamReader(stream))
{
string sqlScript = reader.ReadToEnd();
Console.WriteLine("SQL script generated with blank lines between rows:");
Console.WriteLine(sqlScript);
}
}
}
}
}
```
### See Also
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)
