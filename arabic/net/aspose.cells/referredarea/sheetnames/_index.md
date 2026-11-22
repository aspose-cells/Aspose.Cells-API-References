---
title: "ReferredArea.SheetNames"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. أسماء جميع أوراق العمل التي يشير إليها هذا الكائن"
type: docs
url: /ar/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

أسماء جميع أوراق العمل التي يشير إليها هذا الكائن.

```csharp
public string[] SheetNames { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لإنشاء إشارة صيغة
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // حساب الصيغ للحصول على الإشارات
            workbook.CalculateFormula();

            // الحصول على النطاق المشار إليه من الصيغة في A3
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // عرض خاصية SheetNames
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // إضافة ورقة عمل أخرى وإنشاء إشارة عبر الأوراق
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // احسب الصيغ مرة أخرى
            workbook.CalculateFormula();

            // احصل على المنطقة المشار إليها من الصيغة عبر الأوراق
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // اعرض أسماء الأوراق للإشارة عبر الأوراق
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // احفظ المصنف
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


