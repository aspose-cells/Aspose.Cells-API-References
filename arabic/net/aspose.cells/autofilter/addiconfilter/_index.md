---
title: "AutoFilter.AddIconFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تضيف مرشح أيقونة"
type: docs
url: /ar/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

يضيف مرشح أيقونة.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| iconSetType | IconSetType | نوع مجموعة الأيقونات. |
| iconId | Int32 | معرف الأيقونة. |

### ملاحظات

يدعم فقط إضافة مرشح الأيقونة. لا يدعم التحقق من أي صف مرئي إذا كان المرشح هو مرشح أيقونة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعبئة بيانات عينة في العمود A
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // الحصول على كائن الفلتر التلقائي
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // تعيين نطاق الفلتر التلقائي (A1:A6) باستخدام startRow, startColumn, endRow
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // إضافة مرشح أيقونة إلى العمود الأول (fieldIndex: 0)
                // باستخدام مجموعة أيقونات 3 إشارات ضوئية (IconSetType.TrafficLights31)
                // تصفية للأيقونة الأولى في المجموعة (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // تحديث الفلتر لتطبيق التغييرات
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


