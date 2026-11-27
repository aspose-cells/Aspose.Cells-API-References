---
title: "WorkbookDesigner.SetDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner‑metod. Ställer in datakälla för ett OleDbConnection‑objekt"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(OleDbConnection) {#setdatasource_3}

Anger datakälla för ett OleDbConnection‑objekt.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| anslutning | OleDbConnection | OleDbConnection‑objekt |

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Anger datakälla för ett SqlConnection‑objekt.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| anslutning | SqlConnection | SqlConnection‑objekt |

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Ställer in datakälla för ett [`ICellsDataTable`](../../icellsdatatable/)‑objekt.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSource | String | Namnet på datakällan. |
| cellsDataTable | ICellsDataTable | datatabell. |

### Exempel

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
            // Skapa exempeldata
            List<Customer> customers = new List<Customer>
            {
                new Customer("Thomas Hardy", "120 Hanover Sq., London"),
                new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
            };

            // Skapa arbetsbok och designer
            Workbook workbook = new Workbook();
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Ställ in datakälla med ICellsDataTable
            designer.SetDataSource("Customer", new CustomerDataSource(customers));
            
            // Bearbeta och spara
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

### Se även

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Anger datakälla för ett DataSet‑objekt.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSet | DataSet | DataSet‑objekt |

### Exempel

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
            // Skapa exempel‑DataSet (ersätter OleDb‑anslutning)
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("OrderDetails");
            
            // Lägg till exempelkolumner och data
            dt.Columns.Add("OrderID", typeof(int));
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            
            // Lägg till exempelrader
            dt.Rows.Add(10248, 11, 14.00m);
            dt.Rows.Add(10248, 42, 9.80m);
            dt.Rows.Add(10249, 72, 34.80m);
            
            ds.Tables.Add(dt);

            // Skapa arbetsboksdesigner och ställ in datakälla
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            designer.SetDataSource(ds);

            // Bearbeta och spara
            designer.Process();
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Anger datakälla för ett DataTable‑objekt.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataTable | DataTable | DataTable‑objekt |

### Exempel

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
            // Skapa en arbetsbokdesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();

            // Skapa en datatabell
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID");
            dataTable.Columns.Add("ProductName");

            // Lägg till exempeldata
            dataTable.Rows.Add(1, "Laptop");
            dataTable.Rows.Add(2, "Smartphone");
            dataTable.Rows.Add(3, "Tablet");

            // Ange datakälla
            designer.SetDataSource(dataTable);

            // Bearbeta designern
            designer.Process();

            // Spara arbetsboken
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Anger datakälla för ett DataView‑objekt och binder det till ett datakällnamn.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataSourceName | String | Datakällans namn. |
| dataView | DataView | DataView-objekt. |

### Exempel

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
            // Skapa en ny WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Skapa en exempelarbetsbok med ett kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
            
            // Ställ in arbetsboken i designern
            designer.Workbook = workbook;

            // Skapa exempel-DataTables
            DataTable dt1 = new DataTable("Investment");
            dt1.Columns.Add("Id", typeof(int));
            dt1.Rows.Add(1);

            DataTable dt2 = new DataTable("Remaining");
            dt2.Columns.Add("Id", typeof(int));
            dt2.Rows.Add(2);

            // Ange datakällor med DataView
            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            // Bearbeta designern
            designer.Process();

            // Skriv ut resultatet
            Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Anger datakälla för ett DataView‑objekt.

```csharp
public void SetDataSource(DataView dataView)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataView | DataView | DataView-objekt |

### Exempel

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
            // Skapa WorkbookDesigner‑objekt
            WorkbookDesigner designer = new WorkbookDesigner();

            // Skapa en ny arbetsbok (i verklig användning skulle du ladda en mall)
            designer.Workbook = new Workbook();

            // Skapa exempeldata
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ProductID");
            dt.Columns.Add("ProductName");
            dt.Rows.Add(1, "Chai");
            dt.Rows.Add(2, "Chang");
            dt.Rows.Add(3, "Aniseed Syrup");

            // Skapa DataView från DataTable
            DataView dataView = new DataView(dt);

            // Ange DataView som datakälla
            designer.SetDataSource(dataView);

            // Bearbeta designern
            designer.Process();

            // Spara resultatet
            designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Anger datakälla för ett IDataReader‑objekt.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på datakällans karta. |
| dataReader | IDataReader | IDataReader-objekt |
| rowCount | Int32 | Antalet datarader. Om smartmarkören inte innehåller \"noadd\" måste vi infoga rader enligt radantalet för prestandaskäl och dynamiska upprepade formler. -1 betyder att parametern är oanvänd. |

### Exempel

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
            // Skapa en DataTable som en alternativ datakälla
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
                
                // Demonstrera SetDataSource med String-, IDataReader- och Int32-parametrar
                wd.SetDataSource("Employees", reader, 5);
                wd.Process();
                
                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Anger databindning till en variabel.

```csharp
public void SetDataSource(string variable, object data)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| variabel | String | Variabelnamn skapat med smartmarkör. |
| data | Object | Källdata. |

### Exempel

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

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


