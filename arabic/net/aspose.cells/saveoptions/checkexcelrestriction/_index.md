---
title: "SaveOptions.CheckExcelRestriction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K سيتم قطعها"
type: docs
url: /ar/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

ما إذا كان سيتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عند إدخال قيمة أطول من 32 كيلوبايت، سيتم قطعها.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // تعطيل التحقق من قيود Excel
            workbook.Settings.CheckExcelRestriction = false;

            // الوصول إلى ورقة العمل الأولى والخلايا
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // إنشاء سلسلة أطول من الحد الطبيعي لـ Excel
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // وضع السلسلة الطويلة في الخلية A1
            cells["A1"].PutValue(longString);

            // تكوين خيارات الحفظ لتجاوز القيود
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // احفظ المصنف
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // تحميل الملف المحفوظ مع تعطيل القيود
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // التحقق من الحفاظ على السلسلة الطويلة
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


