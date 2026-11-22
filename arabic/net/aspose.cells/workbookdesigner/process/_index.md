---
title: "WorkbookDesigner.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookDesigner. تعالج العلامات الذكية وتملأ قيم مصدر البيانات"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق المراد معالجته |
| isPreserved | منطقي | صحيح إذا تم الحفاظ على العلامة الذكية غير المعروفة. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام علامات النطاق الذكية. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            
            // إنشاء بيانات عينة في الخلايا
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // إنشاء مصمم دفتر عمل
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // إنشاء مصدر بيانات JSON
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // معالجة نطاق محدد باستخدام العلامات الذكية
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // معالجة النطاق (true = معالجة هذا النطاق فقط)
            designer.Process(range, true);
            
            // حفظ النتيجة
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

```csharp
public void Process()
```

### أمثلة

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل من ملف القالب
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // تحضير مصدر البيانات
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // تعيين مصدر البيانات ومعالجته
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
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

---

## Process(bool) {#process_2}

يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

```csharp
public void Process(bool isPreserved)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isPreserved | منطقي | صحيح إذا تم الحفاظ على العلامة الذكية غير المعروفة. |

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // تهيئة المصنف وتحميل القالب
            Workbook workbook = new Workbook("example.xlsx");
            
            // إنشاء بيانات عينة مباشرةً بدلاً من التحميل من JSON
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // إعداد العلامات الذكية
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // تحضير مصادر البيانات
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // معالجة مصمم المصنف
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // معالجة باستخدام معامل منطقي
            designer.Process(true);
            
            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }

    // فئات بيانات العينة
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

يعالج العلامات الذكية ويملأ قيم مصدر البيانات.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس ورقة العمل. |
| isPreserved | منطقي | صحيح إذا تم الحفاظ على العلامة الذكية غير المعروفة. |

### ملاحظات

هذه الطريقة تعمل على مستوى ورقة العمل.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // تصدير البيانات من ورقة العمل إلى DataTable
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // إنشاء مصمم المصنف وتعيين مصدر البيانات
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // معالجة المصمم باستخدام المعاملات (Int32, Boolean)
            designer.Process(0, true);

            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


