---
title: "WorkbookDesigner.SetDataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner yöntemi. Bir OleDbConnection nesnesinin veri kaynağını ayarlar"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(OleDbConnection) {#setdatasource_3}

Bir OleDbConnection nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bağlantı | OleDbConnection | OleDbConnection nesnesi |

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Bir SqlConnection nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bağlantı | SqlConnection | SqlConnection nesnesi |

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Bir [`ICellsDataTable`](../../icellsdatatable/) nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataSource | String | Veri kaynağının adı. |
| cellsDataTable | ICellsDataTable | veri tablosu. |

### Örnekler

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
            // Örnek veri oluştur
            List<Customer> customers = new List<Customer>
            {
                new Customer("Thomas Hardy", "120 Hanover Sq., London"),
                new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
            };

            // Çalışma kitabı ve tasarımcı oluştur
            Workbook workbook = new Workbook();
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // ICellsDataTable kullanarak veri kaynağını ayarla
            designer.SetDataSource("Customer", new CustomerDataSource(customers));
            
            // İşle ve kaydet
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

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Bir DataSet nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataSet | DataSet | DataSet nesnesi |

### Örnekler

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
            // Örnek DataSet oluştur (OleDb bağlantısını değiştirerek)
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("OrderDetails");
            
            // Örnek sütunları ve verileri ekle
            dt.Columns.Add("OrderID", typeof(int));
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            
            // Örnek satırları ekle
            dt.Rows.Add(10248, 11, 14.00m);
            dt.Rows.Add(10248, 42, 9.80m);
            dt.Rows.Add(10249, 72, 34.80m);
            
            ds.Tables.Add(dt);

            // Çalışma kitabı tasarımcısını oluştur ve veri kaynağını ayarla
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            designer.SetDataSource(ds);

            // İşle ve kaydet
            designer.Process();
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Bir DataTable nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataTable | DataTable | DataTable nesnesi |

### Örnekler

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
            // Bir çalışma kitabı tasarımcısı oluşturun
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();

            // Bir veri tablosu oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID");
            dataTable.Columns.Add("ProductName");

            // Örnek veri ekleyin.
            dataTable.Rows.Add(1, "Laptop");
            dataTable.Rows.Add(2, "Smartphone");
            dataTable.Rows.Add(3, "Tablet");

            // Veri kaynağını ayarla
            designer.SetDataSource(dataTable);

            // Tasarımcıyı işleyin
            designer.Process();

            // Çalışma kitabını kaydedin
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Bir DataView nesnesinin veri kaynağını ayarlar ve onu bir veri kaynağı adına bağlar.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataSourceName | String | Veri kaynağı adı. |
| dataView | DataView | DataView nesnesi. |

### Örnekler

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
            // Yeni bir WorkbookDesigner oluştur
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Bir çalışma sayfası içeren örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
            
            // Çalışma kitabını tasarımcıya ayarla
            designer.Workbook = workbook;

            // Örnek DataTable'lar oluştur
            DataTable dt1 = new DataTable("Investment");
            dt1.Columns.Add("Id", typeof(int));
            dt1.Rows.Add(1);

            DataTable dt2 = new DataTable("Remaining");
            dt2.Columns.Add("Id", typeof(int));
            dt2.Rows.Add(2);

            // DataView kullanarak veri kaynaklarını ayarla
            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            // Tasarımcıyı işleyin
            designer.Process();

            // Sonucu çıktı olarak ver
            Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Bir DataView nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(DataView dataView)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataView | DataView | DataView nesnesi |

### Örnekler

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
            // WorkbookDesigner nesnesi oluştur
            WorkbookDesigner designer = new WorkbookDesigner();

            // Yeni bir çalışma kitabı oluştur (gerçek kullanımda bir şablon yüklersiniz)
            designer.Workbook = new Workbook();

            // Örnek veri oluştur
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ProductID");
            dt.Columns.Add("ProductName");
            dt.Rows.Add(1, "Chai");
            dt.Rows.Add(2, "Chang");
            dt.Rows.Add(3, "Aniseed Syrup");

            // DataTable'dan DataView oluştur
            DataView dataView = new DataView(dt);

            // DataView'i veri kaynağı olarak ayarla
            designer.SetDataSource(dataView);

            // Tasarımcıyı işleyin
            designer.Process();

            // Sonucu kaydet
            designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Bir IDataReader nesnesinin veri kaynağını ayarlar.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Veri kaynağı harita adı. |
| dataReader | IDataReader | IDataReader nesnesi |
| rowCount | Int32 | Veri satırlarının sayısı. Akıllı işaretçi "noadd" içermiyorsa, performans sorunu ve dinamik tekrarlanan formüller için satır sayısına göre satır eklememiz gerekir. -1 parametrenin işe yaramaz olduğunu gösterir. |

### Örnekler

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
            // Alternatif bir veri kaynağı olarak bir DataTable oluşturun
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
                
                // SetDataSource yöntemini String, IDataReader, Int32 parametreleriyle gösterin
                wd.SetDataSource("Employees", reader, 5);
                wd.Process();
                
                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Veri bağlamayı bir değişkene ayarlar.

```csharp
public void SetDataSource(string variable, object data)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değişken | String | Akıllı işaretçi kullanılarak oluşturulan değişken adı. |
| veri | Object | Kaynak veri. |

### Örnekler

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

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


