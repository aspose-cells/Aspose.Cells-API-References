---
title: "Worksheet.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل أو تعين اسم ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

يحصل على أو يضبط اسم ورقة العمل.

```csharp
public string Name { get; set; }
```

### ملاحظات

الحد الأقصى لطول اسم الورقة هو 31. ولا يمكنك تعيين نفس الاسم (بدون حساسية لحالة الأحرف) لورقتين عمل. على سبيل المثال، لا يمكنك تعيين "SheetName1" للورقة الأولى وتعيين "SHEETNAME1" للورقة الثانية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وتعيين اسمها
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // إضافة ورقة عمل جديدة باسم محدد
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // إخراج أسماء جميع أوراق العمل
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // احفظ المصنف
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


