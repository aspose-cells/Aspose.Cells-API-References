##Cells.ImportCustomObjects
Cells method. Imports custom objects
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}
Imports custom objects.
```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown,
int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString,
bool convertStringToNumber)
```
| Parameter | Type | Description |
| --- | --- | --- |
| list | ICollection | The custom object |
| propertyNames | String[] | The property names.If it is null,we will import all properties of the object. |
| isPropertyNameShown | Boolean | Indicates whether the property name will be imported to the first row. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| rowNumber | Int32 | Number of rows to be imported. |
| insertRows | Boolean | Indicates whether extra rows are added to fit data. |
| dateFormatString | String | Date format string for cells. |
| convertStringToNumber | Boolean | Indicates if this method will try to convert string to number. |
### Return Value
Total number of rows imported.
### Remarks
The custom objects should be the same type.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections.Generic;
public class CellsMethodImportCustomObjectsWithICollectionStringBooleanInt3Demo
{
public class Product
{
public string Name { get; set; }
public decimal Price { get; set; }
public int Stock { get; set; }
public DateTime Date { get; set; }
}
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
List<Product> products = new List<Product>
{
new Product { Name = "Apple", Price = 2.99m, Stock = 150, Date = new DateTime(2023, 12, 31) },
new Product { Name = "Orange", Price = 1.99m, Stock = 200, Date = new DateTime(2024, 1, 15) }
};
string[] propertyNames = { "Name", "Price", "Stock", "Date" };
try
{
int importedRows = worksheet.Cells.ImportCustomObjects(
products,
propertyNames,
true,
0,
0,
products.Count,
true,
"yyyy-MM-dd",
true
);
Console.WriteLine($"Successfully imported {importedRows} rows");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ImportCustomObjects: {ex.Message}");
}
workbook.Save("ImportCustomObjectsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}
Imports custom objects.
```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn,
ImportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| list | ICollection | The custom object |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| options | ImportTableOptions | The import options. |
### Return Value
Total number of rows imported.
### Remarks
The custom objects should be the same type.
### Examples
```csharp
using System;
using System.Collections;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class Customer
{
public int CustomerId { get; set; }
public string Name { get; set; }
}
public class CellsMethodImportCustomObjectsWithICollectionInt32Int32ImportTabDemo
{
public static void Run()
{
Workbook wb = new Workbook();
List<Customer> customerList = new List<Customer>();
for (int i = 0; i < 5; i++)
{
customerList.Add(new Customer
{
CustomerId = i,
Name = "Customer" + i
});
}
ImportTableOptions options = new ImportTableOptions
{
IsFieldNameShown = false,
TotalRows = customerList.Count,
InsertRows = true,
DateFormat = "dd/mm/yyyy",
ConvertNumericData = true,
CheckMergedCells = true
};
wb.Worksheets[0].Cells.ImportCustomObjects((ICollection)customerList, 1, 0, options);
wb.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
