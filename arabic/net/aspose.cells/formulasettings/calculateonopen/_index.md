---
title: "FormulaSettings.CalculateOnOpen"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. تشير إلى ما إذا كان التطبيق مطلوبًا منه إجراء حساب كامل عند فتح المصنف"
type: docs
url: /ar/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

يشير إلى ما إذا كان التطبيق مطلوبًا لتنفيذ حساب كامل عند فتح المصنف.

```csharp
public bool CalculateOnOpen { get; set; }
```

### ملاحظات

هذه الخاصية مخصصة فقط لحفظ الإعدادات في ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل مايكروسوفت إكسل) التصرف وفقًا لذلك عند تحميل الملف الناتج. لأسباب تتعلق بالأداء في معظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضع صيغة في الخلية A1 تشير إلى B1
            worksheet.Cells["A1"].Formula = "=B1";
            
            // ضع قيمة في الخلية B1
            worksheet.Cells["B1"].PutValue(10);
            
            // تعطيل حساب الصيغ التلقائي عند الفتح
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // إعادة فتح المصنف المحفوظ
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // تحقق من عدم حساب الصيغة عند الفتح
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // احسب الصيغ يدويًا
            reopenedWorkbook.CalculateFormula();
            
            // تحقق من حساب الصيغة
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


