---
title: "Worksheet.AdvancedFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تقوم بترشيح البيانات باستخدام معايير معقدة"
type: docs
url: /ar/net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

يفلتر البيانات باستخدام معايير معقدة.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isFilter | منطقي | يشير إلى ما إذا كان يتم ترشيح القائمة في الموقع. |
| listRange | String | نطاق القائمة. |
| criteriaRange | String | نطاق المعايير. |
| copyTo | String | النطاق الذي يتم نسخ البيانات إليه. |
| uniqueRecordOnly | منطقي | عرض أو نسخ الصفوف الفريدة فقط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة للترشيح
            // العناوين
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            // المعايير
            worksheet.Cells["A2"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Category");
            worksheet.Cells["C2"].PutValue("Fruits");
            
            // البيانات
            worksheet.Cells["A4"].PutValue("Apple");
            worksheet.Cells["B4"].PutValue("Fruits");
            worksheet.Cells["C4"].PutValue(2.5);
            
            worksheet.Cells["A5"].PutValue("Carrot");
            worksheet.Cells["B5"].PutValue("Vegetables");
            worksheet.Cells["C5"].PutValue(1.2);
            
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B6"].PutValue("Fruits");
            worksheet.Cells["C6"].PutValue(1.8);

            // تطبيق مرشح متقدم (المرشح في الموقع، سجلات فريدة فقط)
            worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);

            // احفظ المصنف
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


