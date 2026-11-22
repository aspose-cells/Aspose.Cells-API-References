---
title: "UnionRange.PutValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. تضع قيمة في النطاق وإذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة تعيين تنسيق أرقام الخلايا"
type: docs
url: /ar/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الرقم للخلية.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | String | قيمة الإدخال |
| isConverted | منطقي | صحيح: تم تحويله إلى نوع بيانات آخر إذا كان مناسبًا. |
| setStyle | منطقي | صحيح: تعيين تنسيق الرقم إلى نمط الخلية عند التحويل إلى نوع بيانات آخر |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق اتحاد يغطي الخلايا A1 إلى B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // استدعِ PutValue مع المعلمات: (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // اعرض معلومات النطاق لإظهار التأثير
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // طبق التنسيق لجعل التأثير مرئيًا
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


