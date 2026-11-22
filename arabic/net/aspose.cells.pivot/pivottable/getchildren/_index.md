---
title: "PivotTable.GetChildren"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تحصل على جداول المحور الفرعية التي تستخدم بيانات هذا PivotTable كمصدر للبيانات"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

يحصل على جداول Pivot الفرعية التي تستخدم بيانات هذا PivotTable كمصدر للبيانات.

```csharp
[Obsolete("Use PivotTable.GetDependentPivotTables() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotTable[] GetChildren()
```

### قيمة الإرجاع

كائن مصفوفة PivotTable

### ملاحظات

ملاحظة: هذه الطريقة أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.GetDependentPivotTables(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetChildrenDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // إنشاء جدول Pivot الرئيسي
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "MainPivotTable");
            PivotTable mainPivotTable = pivotTables[index];
            mainPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            mainPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // إنشاء جدول Pivot فرعي
            index = pivotTables.Add("A1:B4", "E10", "ChildPivotTable");
            PivotTable childPivotTable = pivotTables[index];
            childPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            childPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // إنشاء علاقة عن طريق مشاركة الحقول الأساسية
            foreach (PivotField field in mainPivotTable.BaseFields)
            {
                childPivotTable.BaseFields.Add(field);
            }

            // عرض طريقة GetChildren()
            Console.WriteLine("Child Pivot Tables:");
            foreach (PivotTable child in mainPivotTable.GetChildren())
            {
                Console.WriteLine("Child Pivot Table Name: " + child.Name);
                Console.WriteLine("Child Pivot Table Location: " + child.TableRange1);
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


