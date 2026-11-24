---
title: "WorkbookDesigner.SetDataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Methode. Legt die Datenquelle eines OleDbConnection-Objekts fest"
type: docs
url: /de/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(OleDbConnection) {#setdatasource_3}

Setzt die Datenquelle eines OleDbConnection‑Objekts.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verbindung | OleDbConnection | OleDbConnection-Objekt |

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Setzt die Datenquelle eines SqlConnection‑Objekts.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verbindung | SqlConnection | SqlConnection-Objekt |

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Legt die Datenquelle eines [`ICellsDataTable`](../../icellsdatatable/) Objekts fest.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSource | String | Der Name der Datenquelle. |
| cellsDataTable | ICellsDataTable | Datentabelle. |

### Beispiele

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
            // Erstelle Beispieldaten
            List<Customer> customers = new List<Customer>
            {
                new Customer("Thomas Hardy", "120 Hanover Sq., London"),
                new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
            };

            // Arbeitsmappe und Designer erstellen
            Workbook workbook = new Workbook();
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Datenquelle mit ICellsDataTable festlegen
            designer.SetDataSource("Customer", new CustomerDataSource(customers));
            
            // Verarbeiten und speichern
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

### Siehe auch

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Setzt die Datenquelle eines DataSet‑Objekts.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSet | DataSet | DataSet-Objekt |

### Beispiele

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
            // Beispiel-DataSet erstellen (OleDb-Verbindung ersetzen)
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("OrderDetails");
            
            // Beispielspalten und -daten hinzufügen
            dt.Columns.Add("OrderID", typeof(int));
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            
            // Beispielzeilen hinzufügen
            dt.Rows.Add(10248, 11, 14.00m);
            dt.Rows.Add(10248, 42, 9.80m);
            dt.Rows.Add(10249, 72, 34.80m);
            
            ds.Tables.Add(dt);

            // WorkbookDesigner erstellen und Datenquelle festlegen
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            designer.SetDataSource(ds);

            // Verarbeiten und speichern
            designer.Process();
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Setzt die Datenquelle eines DataTable‑Objekts.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataTable | DataTable | DataTable-Objekt |

### Beispiele

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
            // Erstelle einen WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();

            // Eine Datentabelle erstellen
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID");
            dataTable.Columns.Add("ProductName");

            // Fügen Sie Beispieldaten hinzu
            dataTable.Rows.Add(1, "Laptop");
            dataTable.Rows.Add(2, "Smartphone");
            dataTable.Rows.Add(3, "Tablet");

            // Datenquelle festlegen
            designer.SetDataSource(dataTable);

            // Verarbeite den Designer
            designer.Process();

            // Speichere die Arbeitsmappe
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Setzt die Datenquelle eines DataView‑Objekts und bindet sie an einen Datenquellennamen.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSourceName | String | Name der Datenquelle. |
| dataView | DataView | DataView-Objekt. |

### Beispiele

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
            // Erstelle einen neuen WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Erstelle eine Beispielarbeitsmappe mit einem Arbeitsblatt
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
            
            // Setze das Workbook für den Designer
            designer.Workbook = workbook;

            // Erstelle Beispiel-DataTables
            DataTable dt1 = new DataTable("Investment");
            dt1.Columns.Add("Id", typeof(int));
            dt1.Rows.Add(1);

            DataTable dt2 = new DataTable("Remaining");
            dt2.Columns.Add("Id", typeof(int));
            dt2.Rows.Add(2);

            // Setze Datenquellen mit DataView
            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            // Verarbeite den Designer
            designer.Process();

            // Gib das Ergebnis aus
            Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Setzt die Datenquelle eines DataView‑Objekts.

```csharp
public void SetDataSource(DataView dataView)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataView | DataView | DataView-Objekt |

### Beispiele

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
            // Erstelle WorkbookDesigner‑Objekt
            WorkbookDesigner designer = new WorkbookDesigner();

            // Erstelle ein neues Workbook (bei realer Verwendung würdest du eine Vorlage laden)
            designer.Workbook = new Workbook();

            // Erstelle Beispieldaten
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ProductID");
            dt.Columns.Add("ProductName");
            dt.Rows.Add(1, "Chai");
            dt.Rows.Add(2, "Chang");
            dt.Rows.Add(3, "Aniseed Syrup");

            // DataView aus DataTable erstellen.
            DataView dataView = new DataView(dt);

            // Setze DataView als Datenquelle
            designer.SetDataSource(dataView);

            // Verarbeite den Designer
            designer.Process();

            // Ergebnis speichern
            designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Setzt die Datenquelle eines IDataReader‑Objekts.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Datenquellenzuordnung. |
| dataReader | IDataReader | IDataReader-Objekt |
| rowCount | Int32 | Die Anzahl der Datenzeilen. Wenn der Smart Marker nicht "noadd" enthält, müssen wir Zeilen anhand der Zeilenanzahl einfügen, um Leistungsprobleme und dynamische wiederholte Formeln zu vermeiden. -1 bedeutet, dass der Parameter nutzlos ist. |

### Beispiele

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
            // Erstelle eine DataTable als alternative Datenquelle
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
                
                // Demonstriere SetDataSource mit String-, IDataReader- und Int32-Parametern
                wd.SetDataSource("Employees", reader, 5);
                wd.Process();
                
                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Setzt die Datenbindung zu einer Variablen.

```csharp
public void SetDataSource(string variable, object data)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Variable | String | Variablenname, der mit Smart Marker erstellt wurde. |
| Daten | Object | Quelldaten. |

### Beispiele

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

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


