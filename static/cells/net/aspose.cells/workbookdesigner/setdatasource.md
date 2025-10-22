##WorkbookDesigner.SetDataSource
WorkbookDesigner method. Sets data source of a ICellsDataTable object
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}
Sets data source of a [`ICellsDataTable`](../../icellsdatatable/) object.
```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataSource | String | The name of the data source. |
| cellsDataTable | ICellsDataTable | data table. |
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetDataSourceWithStringICellsDataTableDemo
{
public static void Run()
{
// Create sample data
List<Customer> customers = new List<Customer>
{
new Customer("Thomas Hardy", "120 Hanover Sq., London"),
new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
};
// Create workbook and designer
Workbook workbook = new Workbook();
WorkbookDesigner designer = new WorkbookDesigner(workbook);
// Set data source using ICellsDataTable
designer.SetDataSource("Customer", new CustomerDataSource(customers));
// Process and save
designer.Process();
workbook.Save("output.xlsx");
}
}
public class Customer
{
public string Name { get; set; }
public string Address { get; set; }
public Customer(string name, string address)
{
Name = name;
Address = address;
}
}
public class CustomerDataSource : ICellsDataTable
{
private readonly List<Customer> _customers;
private int _currentRow = -1;
public CustomerDataSource(List<Customer> customers)
{
_customers = customers;
}
public object this[int rowIndex, int columnIndex] =>
columnIndex == 0 ? _customers[rowIndex].Name : _customers[rowIndex].Address;
public object this[int rowIndex] => _customers[rowIndex];
public object this[string columnName] => columnName == "Name" ? _customers[_currentRow].Name : _customers[_currentRow].Address;
public int RowCount => _customers.Count;
public int ColumnCount => 2;
public int Count => _customers.Count;
public string[] Columns => new string[] { "Name", "Address" };
public void BeforeFirst()
{
_currentRow = -1;
}
public bool Next()
{
_currentRow++;
return _currentRow < _customers.Count;
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(DataSet) {#setdatasource}
Sets data source of a DataSet object.
```csharp
public void SetDataSource(DataSet dataSet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataSet | DataSet | DataSet object |
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetDataSourceWithDataSetDemo
{
public static void Run()
{
// Create sample DataSet (replacing OleDb connection)
DataSet ds = new DataSet();
DataTable dt = new DataTable("OrderDetails");
// Add sample columns and data
dt.Columns.Add("OrderID", typeof(int));
dt.Columns.Add("ProductID", typeof(int));
dt.Columns.Add("UnitPrice", typeof(decimal));
// Add sample rows
dt.Rows.Add(10248, 11, 14.00m);
dt.Rows.Add(10248, 42, 9.80m);
dt.Rows.Add(10249, 72, 34.80m);
ds.Tables.Add(dt);
// Create workbook designer and set data source
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = new Workbook();
designer.SetDataSource(ds);
// Process and save
designer.Process();
designer.Workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(DataTable) {#setdatasource_1}
Sets data source of a DataTable object.
```csharp
public void SetDataSource(DataTable dataTable)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | DataTable object |
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetDataSourceWithDataTableDemo
{
public static void Run()
{
// Create a workbook designer
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = new Workbook();
// Create a data table
DataTable dataTable = new DataTable("Products");
dataTable.Columns.Add("ProductID");
dataTable.Columns.Add("ProductName");
// Add sample data
dataTable.Rows.Add(1, "Laptop");
dataTable.Rows.Add(2, "Smartphone");
dataTable.Rows.Add(3, "Tablet");
// Set data source
designer.SetDataSource(dataTable);
// Process the designer
designer.Process();
// Save the workbook
designer.Workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(string, DataView) {#setdatasource_6}
Sets data source of a DataView object and binds it to a data source name.
```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataSourceName | String | Data source name. |
| dataView | DataView | DataView object. |
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetDataSourceWithStringDataViewDemo
{
public static void Run()
{
// Create a new WorkbookDesigner
WorkbookDesigner designer = new WorkbookDesigner();
// Create a sample workbook with a worksheet
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
// Set the workbook to the designer
designer.Workbook = workbook;
// Create sample DataTables
DataTable dt1 = new DataTable("Investment");
dt1.Columns.Add("Id", typeof(int));
dt1.Rows.Add(1);
DataTable dt2 = new DataTable("Remaining");
dt2.Columns.Add("Id", typeof(int));
dt2.Rows.Add(2);
// Set data sources using DataView
designer.SetDataSource("Investment", dt1.DefaultView);
designer.SetDataSource("Remaining", dt2.DefaultView);
// Process the designer
designer.Process();
// Output the result
Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(DataView) {#setdatasource_2}
Sets data source of a DataView object.
```csharp
public void SetDataSource(DataView dataView)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | DataView object |
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetDataSourceWithDataViewDemo
{
public static void Run()
{
// Create WorkbookDesigner object
WorkbookDesigner designer = new WorkbookDesigner();
// Create a new workbook (in real usage you would load a template)
designer.Workbook = new Workbook();
// Create sample data
DataTable dt = new DataTable("Products");
dt.Columns.Add("ProductID");
dt.Columns.Add("ProductName");
dt.Rows.Add(1, "Chai");
dt.Rows.Add(2, "Chang");
dt.Rows.Add(3, "Aniseed Syrup");
// Create DataView from DataTable
DataView dataView = new DataView(dt);
// Set DataView as data source
designer.SetDataSource(dataView);
// Process the designer
designer.Process();
// Save the result
designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(string, IDataReader, int) {#setdatasource_7}
Sets data source of a IDataReader object.
```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The data source map name. |
| dataReader | IDataReader | IDataReader object |
| rowCount | Int32 | The number of the data rows. If the smart marker does not contains "noadd", we have to insert rows by the row count for performance issue and dynamic repeated formulas. -1 means the param is useless. |
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetDataSourceWithStringIDataReaderInt32Demo
{
public static void Run()
{
// Create a DataTable as an alternative data source
DataTable table = new DataTable("Employees");
table.Columns.Add("ID", typeof(int));
table.Columns.Add("Name", typeof(string));
table.Rows.Add(1, "John Doe");
table.Rows.Add(2, "Jane Smith");
table.Rows.Add(3, "Mike Johnson");
table.Rows.Add(4, "Sarah Williams");
table.Rows.Add(5, "David Brown");
using (IDataReader reader = table.CreateDataReader())
{
WorkbookDesigner wd = new WorkbookDesigner();
Workbook wb = new Workbook();
wd.Workbook = wb;
// Demonstrate SetDataSource with String, IDataReader, Int32 parameters
wd.SetDataSource("Employees", reader, 5);
wd.Process();
wb.Save("output.xlsx");
}
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(string, object) {#setdatasource_8}
Sets data binding to a variable.
```csharp
public void SetDataSource(string variable, object data)
```
| Parameter | Type | Description |
| --- | --- | --- |
| variable | String | Variable name created using smart marker. |
| data | Object | Source data. |
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodSetDataSourceWithStringObjectDemo
{
public static void Run()
{
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = new Workbook();
Worksheet worksheet = designer.Workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("&=$Person.Name");
worksheet.Cells["C1"].PutValue("&=$Person.Wife.Name");
List<Person> persons = new List<Person>
{
new Person("simon", 30) { Wife = new Wife("simon.wife", 30) },
new Person("Johnson", 30) { Wife = new Wife("Johnson.wife", 30) }
};
designer.SetDataSource("Person", persons);
designer.Process();
Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
Console.WriteLine("C1: " + worksheet.Cells["C1"].StringValue);
Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
}
}
public class Person
{
public string Name { get; set; }
public int Age { get; set; }
public Wife Wife { get; set; }
public Person(string name, int age)
{
Name = name;
Age = age;
}
}
public class Wife
{
public string Name { get; set; }
public int Age { get; set; }
public Wife(string name, int age)
{
Name = name;
Age = age;
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(OleDbConnection) {#setdatasource_3}
Sets data source of a OleDbConnection object.
```csharp
public void SetDataSource(OleDbConnection connection)
```
| Parameter | Type | Description |
| --- | --- | --- |
| connection | OleDbConnection | OleDbConnection object |
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetDataSource(SqlConnection) {#setdatasource_4}
Sets data source of a SqlConnection object.
```csharp
public void SetDataSource(SqlConnection connection)
```
| Parameter | Type | Description |
| --- | --- | --- |
| connection | SqlConnection | SqlConnection object |
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
