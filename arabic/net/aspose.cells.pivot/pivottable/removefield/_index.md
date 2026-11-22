---
title: "PivotTable.RemoveField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. يزيل حقلًا من منطقة حقل محددة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

يزيل حقلًا من منطقة الحقول المحددة

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | PivotFieldType | نوع منطقة الحقول. |
| fieldName | String | الاسم في الحقول الأساسية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // إزالة الحقل "c" من منطقة البيانات
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // حساب بيانات جدول المحور
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

يزيل حقلًا من منطقة المحور المحددة.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | PivotFieldType | نوع منطقة الحقول. |
| baseFieldIndex | Int32 | فهرس الحقل في الحقول الأساسية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // إزالة حقل الصف (الفهرس 0) من جدول المحور
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

إزالة الحقل من منطقة الحقل المحددة

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | PivotFieldType | نوع منطقة الحقول. |
| pivotField | PivotField | الحقل في الحقول الأساسية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // إزالة حقل عمود من جدول المحور
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // إزالة حقل بيانات من جدول المحور
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // احفظ المصنف
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


