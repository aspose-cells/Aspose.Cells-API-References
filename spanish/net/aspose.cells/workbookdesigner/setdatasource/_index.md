---
title: "WorkbookDesigner.SetDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookDesigner. Establece el origen de datos de un objeto OleDbConnection"
type: docs
url: /es/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(OleDbConnection) {#setdatasource_3}

Establece la fuente de datos de un objeto OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| conexión | OleDbConnection | objeto OleDbConnection |

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Establece la fuente de datos de un objeto SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| conexión | SqlConnection | objeto SqlConnection |

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Establece el origen de datos de un objeto [`ICellsDataTable`](../../icellsdatatable/).

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataSource | String | El nombre del origen de datos. |
| cellsDataTable | ICellsDataTable | tabla de datos. |

### Ejemplos

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
            // Crear datos de ejemplo
            List<Customer> customers = new List<Customer>
            {
                new Customer("Thomas Hardy", "120 Hanover Sq., London"),
                new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
            };

            // Crear libro de trabajo y diseñador
            Workbook workbook = new Workbook();
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Establecer origen de datos usando ICellsDataTable
            designer.SetDataSource("Customer", new CustomerDataSource(customers));
            
            // Procesar y guardar
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

### Ver también

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Establece la fuente de datos de un objeto DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataSet | DataSet | Objeto DataSet |

### Ejemplos

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
            // Crear DataSet de muestra (reemplazando la conexión OleDb)
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("OrderDetails");
            
            // Agregar columnas y datos de muestra
            dt.Columns.Add("OrderID", typeof(int));
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            
            // Agregar filas de muestra
            dt.Rows.Add(10248, 11, 14.00m);
            dt.Rows.Add(10248, 42, 9.80m);
            dt.Rows.Add(10249, 72, 34.80m);
            
            ds.Tables.Add(dt);

            // Crear diseñador de libro de trabajo y establecer origen de datos
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            designer.SetDataSource(ds);

            // Procesar y guardar
            designer.Process();
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Establece la fuente de datos de un objeto DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataTable | DataTable | Objeto DataTable |

### Ejemplos

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
            // Crear un diseñador de libros de trabajo
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();

            // Crear una tabla de datos
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID");
            dataTable.Columns.Add("ProductName");

            // Agregar datos de ejemplo
            dataTable.Rows.Add(1, "Laptop");
            dataTable.Rows.Add(2, "Smartphone");
            dataTable.Rows.Add(3, "Tablet");

            // Establecer origen de datos
            designer.SetDataSource(dataTable);

            // Procesar el diseñador
            designer.Process();

            // Guarda el libro de trabajo
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Establece la fuente de datos de un objeto DataView y lo vincula a un nombre de fuente de datos.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataSourceName | String | Nombre del origen de datos. |
| dataView | DataView | Objeto DataView. |

### Ejemplos

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
            // Crear un nuevo WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Crear un libro de trabajo de muestra con una hoja de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
            
            // Establecer el libro de trabajo en el diseñador
            designer.Workbook = workbook;

            // Crear DataTables de muestra
            DataTable dt1 = new DataTable("Investment");
            dt1.Columns.Add("Id", typeof(int));
            dt1.Rows.Add(1);

            DataTable dt2 = new DataTable("Remaining");
            dt2.Columns.Add("Id", typeof(int));
            dt2.Rows.Add(2);

            // Establecer orígenes de datos usando DataView
            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            // Procesar el diseñador
            designer.Process();

            // Mostrar el resultado
            Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Establece la fuente de datos de un objeto DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataView | DataView | Objeto DataView |

### Ejemplos

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
            // Crear objeto WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();

            // Crear un nuevo libro de trabajo (en uso real cargarías una plantilla)
            designer.Workbook = new Workbook();

            // Crear datos de ejemplo
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ProductID");
            dt.Columns.Add("ProductName");
            dt.Rows.Add(1, "Chai");
            dt.Rows.Add(2, "Chang");
            dt.Rows.Add(3, "Aniseed Syrup");

            // Crear DataView a partir de DataTable
            DataView dataView = new DataView(dt);

            // Establecer DataView como origen de datos
            designer.SetDataSource(dataView);

            // Procesar el diseñador
            designer.Process();

            // Guardar el resultado
            designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Establece la fuente de datos de un objeto IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del mapa de origen de datos. |
| dataReader | IDataReader | objeto IDataReader |
| rowCount | Int32 | El número de filas de datos. Si el marcador inteligente no contiene "noadd", debemos insertar filas según el recuento de filas por problemas de rendimiento y fórmulas repetidas dinámicas. -1 significa que el parámetro es inútil. |

### Ejemplos

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
            // Crear un DataTable como fuente de datos alternativa
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
                
                // Demostrar SetDataSource con parámetros String, IDataReader, Int32
                wd.SetDataSource("Employees", reader, 5);
                wd.Process();
                
                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Establece el enlace de datos a una variable.

```csharp
public void SetDataSource(string variable, object data)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| variable | String | Nombre de variable creado usando marcador inteligente. |
| datos | Objeto | Datos de origen. |

### Ejemplos

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

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


