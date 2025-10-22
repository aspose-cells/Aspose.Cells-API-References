##ICellsDataTable.Item
ICellsDataTable property. Gets the data stored in the column specified by index
## ICellsDataTable indexer (1 of 2)
Gets the data stored in the column specified by index.
```csharp
public object this[int columnIndex] { get; }
```
| Parameter | Description |
| --- | --- |
| columnIndex | The zero-based index of the column. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ICellsDataTablePropertyItemDemo
{
public static void Run()
{
// Create custom ICellsDataTable with sample data
ICellsDataTable dataTable = new SampleDataTable();
// Reset cursor position
dataTable.BeforeFirst();
Console.WriteLine("Reading data using Item property:");
while (dataTable.Next())
{
// Access values by column index
Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");
// Access values by column name
Console.WriteLine($"Product: {dataTable["Product"]}, Price: {dataTable["Price"]}, Stock: {dataTable["Stock"]}\n");
}
}
}
internal class SampleDataTable : ICellsDataTable
{
private readonly string[] columns = { "Product", "Price", "Stock" };
private readonly object[][] data =
{
new object[] { "Laptop", 999.99, 15 },
new object[] { "Phone", 699.99, 25 },
new object[] { "Tablet", 299.99, 50 }
};
private int currentRow = -1;
public string[] Columns => columns;
public int Count => data.Length;
public object this[int columnIndex] => data[currentRow][columnIndex];
public object this[string columnName] => data[currentRow][Array.IndexOf(columns, columnName)];
public void BeforeFirst() => currentRow = -1;
public bool Next() => ++currentRow < data.Length;
}
}
```
### See Also
* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ICellsDataTable indexer (2 of 2)
Gets the data stored in the column specified by column name.
```csharp
public object this[string columnName] { get; }
```
| Parameter | Description |
| --- | --- |
| columnName | The column name. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ICellsDataTablePropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data into cells
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(999.99);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(499.99);
// Export data range to ICellsDataTable with explicit cast
ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);
// Move to before first record
dataTable.BeforeFirst();
Console.WriteLine("Reading data table values:");
while (dataTable.Next())
{
// Access Item property using column names (indexer)
string product = dataTable["Product"].ToString();
double price = Convert.ToDouble(dataTable["Price"]);
Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
}
// Save the workbook
workbook.Save("ItemPropertyDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
