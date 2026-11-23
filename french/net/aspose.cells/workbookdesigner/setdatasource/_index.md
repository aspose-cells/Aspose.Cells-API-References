---
title: "WorkbookDesigner.SetDataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookDesigner. Définit la source de données d'un objet OleDbConnection"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(OleDbConnection) {#setdatasource_3}

Définit la source de données d'un objet OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connexion | OleDbConnection | objet OleDbConnection |

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Définit la source de données d'un objet SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connexion | SqlConnection | objet SqlConnection |

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Définit la source de données d'un objet [`ICellsDataTable`](../../icellsdatatable/).

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataSource | String | Le nom de la source de données. |
| cellsDataTable | ICellsDataTable | table de données. |

### Exemples

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
            // Créer des données d'exemple
            List<Customer> customers = new List<Customer>
            {
                new Customer("Thomas Hardy", "120 Hanover Sq., London"),
                new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
            };

            // Créer le classeur et le concepteur
            Workbook workbook = new Workbook();
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Définir la source de données en utilisant ICellsDataTable
            designer.SetDataSource("Customer", new CustomerDataSource(customers));
            
            // Traiter et enregistrer
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

### Voir aussi

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Définit la source de données d'un objet DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataSet | DataSet | Objet DataSet |

### Exemples

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
            // Créer un DataSet d'exemple (remplaçant la connexion OleDb)
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("OrderDetails");
            
            // Ajouter des colonnes et des données d'exemple
            dt.Columns.Add("OrderID", typeof(int));
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            
            // Ajouter des lignes d'exemple
            dt.Rows.Add(10248, 11, 14.00m);
            dt.Rows.Add(10248, 42, 9.80m);
            dt.Rows.Add(10249, 72, 34.80m);
            
            ds.Tables.Add(dt);

            // Créer le concepteur de classeur et définir la source de données
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            designer.SetDataSource(ds);

            // Traiter et enregistrer
            designer.Process();
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Définit la source de données d'un objet DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataTable | DataTable | Objet DataTable |

### Exemples

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
            // Créer un concepteur de classeur
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();

            // Créer une table de données
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID");
            dataTable.Columns.Add("ProductName");

            // Ajoutez des données d'exemple
            dataTable.Rows.Add(1, "Laptop");
            dataTable.Rows.Add(2, "Smartphone");
            dataTable.Rows.Add(3, "Tablet");

            // Définir la source de données
            designer.SetDataSource(dataTable);

            // Traiter le concepteur
            designer.Process();

            // Enregistrez le classeur
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Définit la source de données d'un objet DataView et l'associe à un nom de source de données.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataSourceName | String | Nom de la source de données. |
| dataView | DataView | Objet DataView. |

### Exemples

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
            // Créer un nouveau WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Créer un classeur d'exemple avec une feuille de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
            
            // Définir le classeur dans le concepteur
            designer.Workbook = workbook;

            // Créer des DataTables d'exemple
            DataTable dt1 = new DataTable("Investment");
            dt1.Columns.Add("Id", typeof(int));
            dt1.Rows.Add(1);

            DataTable dt2 = new DataTable("Remaining");
            dt2.Columns.Add("Id", typeof(int));
            dt2.Rows.Add(2);

            // Définir les sources de données en utilisant DataView
            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            // Traiter le concepteur
            designer.Process();

            // Afficher le résultat
            Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Définit la source de données d'un objet DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataView | DataView | Objet DataView |

### Exemples

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
            // Créer l'objet WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();

            // Créer un nouveau classeur (dans une utilisation réelle, vous chargeriez un modèle)
            designer.Workbook = new Workbook();

            // Créer des données d'exemple
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ProductID");
            dt.Columns.Add("ProductName");
            dt.Rows.Add(1, "Chai");
            dt.Rows.Add(2, "Chang");
            dt.Rows.Add(3, "Aniseed Syrup");

            // Créer DataView à partir de DataTable
            DataView dataView = new DataView(dt);

            // Définir DataView comme source de données
            designer.SetDataSource(dataView);

            // Traiter le concepteur
            designer.Process();

            // Enregistrer le résultat
            designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Définit la source de données d'un objet IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de la carte de source de données. |
| dataReader | IDataReader | Objet IDataReader |
| rowCount | Int32 | Le nombre de lignes de données. Si le smart marker ne contient pas "noadd", nous devons insérer des lignes selon le nombre de lignes pour des problèmes de performance et des formules répétées dynamiques. -1 signifie que le paramètre est inutile. |

### Exemples

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
            // Créer un DataTable comme source de données alternative
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
                
                // Démontrer SetDataSource avec les paramètres String, IDataReader, Int32
                wd.SetDataSource("Employees", reader, 5);
                wd.Process();
                
                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Définit la liaison de données à une variable.

```csharp
public void SetDataSource(string variable, object data)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| variable | String | Nom de variable créé à l'aide du smart marker. |
| données | Object | Données source. |

### Exemples

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

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


