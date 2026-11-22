---
title: "WorkbookSettings.CheckExcelRestriction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحدد ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الخلايا أو الكائنات المرتبطة. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عند إدخال قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValuestring، إذا كانت هذه الخاصية true ستحصل على Exception. إذا كانت الخاصية false سنقبل قيمة النص التي أدخلتها كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة الكاملة إلى صيغ ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ."
type: docs
url: /ar/net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت false، سنقبل قيمة النص المدخلة كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة إلى صيغ ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعطيل التحقق من قيود Excel
            workbook.Settings.CheckExcelRestriction = false;
            
            // إدراج سلسلة تتجاوز حدود Excel العادية
            string longString = new string('a', 40000);
            workbook.Worksheets[0].Cells["A1"].PutValue(longString);
            
            // احفظ وأعد التحميل للتحقق من تجاوز القيود
            string tempFile = Guid.NewGuid().ToString() + ".txt";
            workbook.Save(tempFile, new TxtSaveOptions());
            
            Workbook loadedWorkbook = new Workbook(tempFile, new LoadOptions { CheckExcelRestriction = false });
            Console.WriteLine("String length: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue.Length);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


