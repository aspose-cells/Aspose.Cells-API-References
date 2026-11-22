---
title: "TimelineCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TimelineCollection. أضف مخططًا زمنيًا جديدًا باستخدام PivotTable كمصدر للبيانات"
type: docs
url: /ar/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر للبيانات

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس إضافة Timeline الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // إضافة timeline متصل بجدول pivot
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // احفظ دفتر العمل
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر للبيانات

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| destCellName | String | اسم الخلية في الزاوية العلوية اليسرى لنطاق Timeline. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس إضافة Timeline الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // إضافة جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // إضافة timeline متصل بجدول pivot
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // احفظ المصنف
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر للبيانات

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس إضافة Timeline الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // إضافة جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة عنصر تحكم timeline
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر للبيانات

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| destCellName | String | اسم الخلية في الزاوية العلوية اليسرى لنطاق Timeline. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس إضافة Timeline الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // تحديث بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // العثور على فهرس الحقل الأساسي لحقل "Date"
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // إضافة timeline باستخدام الفهرس الموجود
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // حفظ النتيجة
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر للبيانات

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس إضافة Timeline الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // إضافة حقول pivot
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // إضافة timeline باستخدام جدول pivot
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // احفظ المصنف
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر للبيانات

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| destCellName | String | اسم الخلية في الزاوية العلوية اليسرى لنطاق Timeline. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس إضافة Timeline الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // إضافة timeline باستخدام جدول pivot كمصدر بيانات
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


