---
title: "WorkbookDesigner.SetDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookDesigner. Imposta la fonte dati di un oggetto OleDbConnection"
type: docs
url: /it/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(OleDbConnection) {#setdatasource_3}

Imposta l'origine dati di un oggetto OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connessione | OleDbConnection | oggetto OleDbConnection |

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Imposta l'origine dati di un oggetto SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connessione | SqlConnection | oggetto SqlConnection |

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Imposta la fonte dati di un oggetto [`ICellsDataTable`](../../icellsdatatable/).

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSource | String | Il nome della fonte dati. |
| cellsDataTable | ICellsDataTable | tabella dei dati. |

### Esempi

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
            // Crea dati di esempio
            List<Customer> customers = new List<Customer>
            {
                new Customer("Thomas Hardy", "120 Hanover Sq., London"),
                new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
            };

            // Crea la cartella di lavoro e il designer
            Workbook workbook = new Workbook();
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Imposta la fonte dati usando ICellsDataTable
            designer.SetDataSource("Customer", new CustomerDataSource(customers));
            
            // Elabora e salva
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

### Vedi anche

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Imposta l'origine dati di un oggetto DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSet | DataSet | oggetto DataSet |

### Esempi

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
            // Crea un DataSet di esempio (sostituendo la connessione OleDb)
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("OrderDetails");
            
            // Aggiungi colonne e dati di esempio
            dt.Columns.Add("OrderID", typeof(int));
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            
            // Aggiungi righe di esempio
            dt.Rows.Add(10248, 11, 14.00m);
            dt.Rows.Add(10248, 42, 9.80m);
            dt.Rows.Add(10249, 72, 34.80m);
            
            ds.Tables.Add(dt);

            // Crea il designer della cartella di lavoro e imposta la fonte dati
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            designer.SetDataSource(ds);

            // Elabora e salva
            designer.Process();
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Imposta l'origine dati di un oggetto DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataTable | DataTable | oggetto DataTable |

### Esempi

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
            // Crea un designer di cartella di lavoro
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();

            // Crea una tabella dati
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID");
            dataTable.Columns.Add("ProductName");

            // Aggiungi dati di esempio
            dataTable.Rows.Add(1, "Laptop");
            dataTable.Rows.Add(2, "Smartphone");
            dataTable.Rows.Add(3, "Tablet");

            // Imposta la fonte dati
            designer.SetDataSource(dataTable);

            // Elabora il designer
            designer.Process();

            // Salva la cartella di lavoro
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Imposta l'origine dati di un oggetto DataView e lo associa a un nome di origine dati.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataSourceName | String | Nome della fonte dati. |
| dataView | DataView | oggetto DataView. |

### Esempi

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
            // Crea un nuovo WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Crea un workbook di esempio con un foglio di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
            
            // Imposta il workbook nel designer
            designer.Workbook = workbook;

            // Crea DataTables di esempio
            DataTable dt1 = new DataTable("Investment");
            dt1.Columns.Add("Id", typeof(int));
            dt1.Rows.Add(1);

            DataTable dt2 = new DataTable("Remaining");
            dt2.Columns.Add("Id", typeof(int));
            dt2.Rows.Add(2);

            // Imposta le fonti dati usando DataView
            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            // Elabora il designer
            designer.Process();

            // Restituisci il risultato
            Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Imposta l'origine dati di un oggetto DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataView | DataView | oggetto DataView |

### Esempi

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
            // Crea l'oggetto WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();

            // Crea un nuovo workbook (in un utilizzo reale dovresti caricare un modello)
            designer.Workbook = new Workbook();

            // Crea dati di esempio
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ProductID");
            dt.Columns.Add("ProductName");
            dt.Rows.Add(1, "Chai");
            dt.Rows.Add(2, "Chang");
            dt.Rows.Add(3, "Aniseed Syrup");

            // Crea DataView da DataTable
            DataView dataView = new DataView(dt);

            // Imposta DataView come fonte dati
            designer.SetDataSource(dataView);

            // Elabora il designer
            designer.Process();

            // Salva il risultato
            designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Imposta l'origine dati di un oggetto IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della mappa della fonte dati. |
| dataReader | IDataReader | oggetto IDataReader |
| rowCount | Int32 | Il numero delle righe di dati. Se lo smart marker non contiene "noadd", dobbiamo inserire righe in base al conteggio delle righe per motivi di prestazioni e formule ripetute dinamiche. -1 indica che il parametro è inutile. |

### Esempi

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
            // Crea un DataTable come fonte dati alternativa
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
                
                // Dimostra SetDataSource con parametri String, IDataReader, Int32
                wd.SetDataSource("Employees", reader, 5);
                wd.Process();
                
                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Imposta il binding dei dati a una variabile.

```csharp
public void SetDataSource(string variable, object data)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| variabile | String | Nome della variabile creato usando lo smart marker. |
| dati | Object | Dati di origine. |

### Esempi

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

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


