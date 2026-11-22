---
title: "Name.SetRefersTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Name. تعيين مرجع هذا Name"
type: docs
url: /ar/net/aspose.cells/name/setrefersto/
---
## Name.SetRefersTo method

اضبط إشارة هذا الاسم.

```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| refersTo | String | المرجع. |
| isR1C1 | منطقي | ما إذا كان المرجع بصيغة R1C1. |
| isLocal | منطقي | ما إذا كان المرجع منسقًا حسب الإعدادات الإقليمية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodSetRefersToWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى الخلايا
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // إنشاء نطاق مسمى
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];

            try
            {
                // استدعِ SetRefersTo مع معلمات (String, Boolean, Boolean)
                namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);

                // اعرض النتيجة
                Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");

                // تحقق باستخدام النطاق المسمى في صيغة
                worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
                workbook.CalculateFormula();

                Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


