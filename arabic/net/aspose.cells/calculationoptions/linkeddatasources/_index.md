---
title: "CalculationOptions.LinkedDataSources"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. تحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ"
type: docs
url: /ar/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### ملاحظات

مثل [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/)، يمكنك هنا تحديد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ التي سيتم حسابها، خاصةً تلك المستخدمة في الدالة INDIRECT. بالنسبة لتلك الروابط الخارجية المستخدمة في الدالة INDIRECT، لا تُعتبر جزءًا من الروابط الخارجية للمصنف ولا يمكن تحديثها بواسطة [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). يتم تحديد تطابق تلك المصنفات مع الروابط الخارجية بواسطة [`FileName`](../../workbook/filename/) و[`DataSource`](../../externallink/datasource/). لذا يرجى التأكد من أن [`FileName`](../../workbook/filename/) قد تم تحديده بالقيمة المناسبة (عادةً يجب أن تكون نفس القيمة المقابلة لـ [`DataSource`](../../externallink/datasource/)) لكل مصنف حتى يمكن ربطها كما هو متوقع.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف خارجي يحتوي على بيانات
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // إضافة نطاقات مسماة في المصنف الخارجي
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // إنشاء المصنف الرئيسي
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // تعيين صيغ تشير إلى المصنف الخارجي
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // احسب الصيغ باستخدام LinkedDataSources
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


