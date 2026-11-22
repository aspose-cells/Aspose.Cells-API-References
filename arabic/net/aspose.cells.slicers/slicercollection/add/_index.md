---
title: "SlicerCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SlicerCollection. أضف مقطعًا جديدًا باستخدام PivotTable كمصدر للبيانات"
type: docs
url: /ar/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // إضافة مقطع
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Fruit");
            cells["B1"].PutValue("Quantity");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(50);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(30);

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة مقطع
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivotTable, 20, 12, "fruit");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // إضافة جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // أضف مقطعًا لجدول المحور
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // إضافة مقطع
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // إضافة حقول pivot
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة مقطع
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // احفظ المصنف
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| محور | PivotTable | كائن PivotTable |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // إضافة مقطع
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // احفظ المصنف
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

إضافة Slicer جديد باستخدام ListObjet كمصدر بيانات

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الجدول | ListObject | كائن ListObject |
| فهرس | Int32 | فهرس ListColumn في ListObject.ListColumns |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء بيانات تجريبية وكائن قائمة
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // أضف مقطعًا لكائن القائمة - ملاحظة: Slicers.Add تُعيد فهرسًا من نوع int
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // احفظ المصنف
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

إضافة Slicer جديد باستخدام ListObjet كمصدر بيانات

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الجدول | ListObject | كائن ListObject |
| listColumn | ListColumn | الـ ListColumn في ListObject.ListColumns |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");

            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, table.ListColumns[1], "I38");

            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells.SetColumnWidth(1, 20);

            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

إضافة Slicer جديد باستخدام ListObjet كمصدر بيانات

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الجدول | ListObject | كائن ListObject |
| listColumn | ListColumn | الـ ListColumn في ListObject.ListColumns |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الـ Slicer. |

### قيمة الإرجاع

فهرس الـ Slicer الجديد المضاف

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية للجدول
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue("CatA");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue("CatB");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue("CatA");
            
            // إنشاء نطاق الجدول
            int endRow = 4;
            string startCell = "A1";
            string endCell = $"B{endRow}";
            
            // أضف جدولًا إلى ورقة العمل باستخدام التحميل الزائد الصحيح
            int tableIndex = sheet.ListObjects.Add(startCell, endCell, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // أضف مقطعًا لعمود الفئة في الموضع (الصف 6، العمود 1)
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(table, table.ListColumns[1], 6, 1);
            
            // حفظ النتيجة
            workbook.Save("SlicerOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


