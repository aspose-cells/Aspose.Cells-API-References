---
title: "WorkbookDesigner.SetDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookDesigner. تعيين مصدر البيانات لكائن OleDbConnection."
type: docs
url: /ar/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(OleDbConnection) {#setdatasource_3}

يضبط مصدر البيانات لكائن OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الاتصال | OleDbConnection | كائن OleDbConnection |

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

يضبط مصدر البيانات لكائن SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الاتصال | SqlConnection | كائن SqlConnection |

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

تعيين مصدر البيانات لكائن [`ICellsDataTable`](../../icellsdatatable/).

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataSource | String | اسم مصدر البيانات. |
| cellsDataTable | ICellsDataTable | جدول البيانات. |

### أمثلة

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
            // إنشاء بيانات نموذجية
            List<Customer> customers = new List<Customer>
            {
                new Customer("Thomas Hardy", "120 Hanover Sq., London"),
                new Customer("Paolo Accorti", "Via Monte Bianco 34, Torino")
            };

            // إنشاء مصنف ومصمم
            Workbook workbook = new Workbook();
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // تعيين مصدر البيانات باستخدام ICellsDataTable
            designer.SetDataSource("Customer", new CustomerDataSource(customers));
            
            // معالجة وحفظ
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

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

يضبط مصدر البيانات لكائن DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataSet | DataSet | كائن DataSet |

### أمثلة

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
            // إنشاء DataSet تجريبي (استبدال اتصال OleDb)
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("OrderDetails");
            
            // إضافة أعمدة وبيانات تجريبية
            dt.Columns.Add("OrderID", typeof(int));
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            
            // إضافة صفوف تجريبية
            dt.Rows.Add(10248, 11, 14.00m);
            dt.Rows.Add(10248, 42, 9.80m);
            dt.Rows.Add(10249, 72, 34.80m);
            
            ds.Tables.Add(dt);

            // إنشاء مصمم المصنف وتعيين مصدر البيانات
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            designer.SetDataSource(ds);

            // معالجة وحفظ
            designer.Process();
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

يضبط مصدر البيانات لكائن DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataTable | DataTable | كائن DataTable |

### أمثلة

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
            // إنشاء مصمم مصنف
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();

            // إنشاء جدول بيانات
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID");
            dataTable.Columns.Add("ProductName");

            // أضف بيانات تجريبية
            dataTable.Rows.Add(1, "Laptop");
            dataTable.Rows.Add(2, "Smartphone");
            dataTable.Rows.Add(3, "Tablet");

            // تعيين مصدر البيانات
            designer.SetDataSource(dataTable);

            // معالجة المصمم
            designer.Process();

            // احفظ المصنف
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

يضبط مصدر البيانات لكائن DataView ويربطه باسم مصدر البيانات.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataSourceName | String | اسم مصدر البيانات. |
| dataView | DataView | كائن DataView. |

### أمثلة

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
            // إنشاء WorkbookDesigner جديد
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // إنشاء دفتر عمل تجريبي مع ورقة عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("&=$Remaining.Id");
            
            // تعيين دفتر العمل للمصمم
            designer.Workbook = workbook;

            // إنشاء DataTables تجريبية
            DataTable dt1 = new DataTable("Investment");
            dt1.Columns.Add("Id", typeof(int));
            dt1.Rows.Add(1);

            DataTable dt2 = new DataTable("Remaining");
            dt2.Columns.Add("Id", typeof(int));
            dt2.Rows.Add(2);

            // تعيين مصادر البيانات باستخدام DataView
            designer.SetDataSource("Investment", dt1.DefaultView);
            designer.SetDataSource("Remaining", dt2.DefaultView);

            // معالجة المصمم
            designer.Process();

            // أخرج النتيجة.
            Console.WriteLine(workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

يضبط مصدر البيانات لكائن DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataView | DataView | كائن DataView |

### أمثلة

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
            // إنشاء كائن WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();

            // إنشاء دفتر عمل جديد (في الاستخدام الفعلي ستقوم بتحميل قالب)
            designer.Workbook = new Workbook();

            // إنشاء بيانات نموذجية
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ProductID");
            dt.Columns.Add("ProductName");
            dt.Rows.Add(1, "Chai");
            dt.Rows.Add(2, "Chang");
            dt.Rows.Add(3, "Aniseed Syrup");

            // إنشاء DataView من DataTable
            DataView dataView = new DataView(dt);

            // تعيين DataView كمصدر للبيانات
            designer.SetDataSource(dataView);

            // معالجة المصمم
            designer.Process();

            // حفظ النتيجة
            designer.Workbook.Save("WorkbookDesignerWithDataView.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

يضبط مصدر البيانات لكائن IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم خريطة مصدر البيانات. |
| dataReader | IDataReader | كائن IDataReader |
| rowCount | Int32 | عدد صفوف البيانات. إذا لم يحتوي العلامة الذكية على "noadd"، يجب علينا إدراج الصفوف حسب عدد الصفوف لأسباب تتعلق بالأداء والصيغ المتكررة الديناميكية. -1 يعني أن المعامل غير مفيد. |

### أمثلة

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
            // إنشاء DataTable كمصدر بيانات بديل
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
                
                // عرض SetDataSource مع معلمات String, IDataReader, Int32
                wd.SetDataSource("Employees", reader, 5);
                wd.Process();
                
                wb.Save("output.xlsx");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

يضبط ربط البيانات إلى متغير.

```csharp
public void SetDataSource(string variable, object data)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| متغير | String | اسم المتغير تم إنشاؤه باستخدام العلامة الذكية. |
| بيانات | Object | بيانات المصدر. |

### أمثلة

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

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


