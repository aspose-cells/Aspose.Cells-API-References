---
title: "InsertOptions.UpdateReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية InsertOptions. تشير إلى ما إذا كانت الإشارات في أوراق عمل أخرى سيتم تحديثها"
type: docs
url: /ar/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

يشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها.

```csharp
public bool UpdateReference { get; set; }
```

### ملاحظات

بدءًا من الإصدار 26.7 نضبط القيمة الافتراضية لهذه الخاصية إلى true.

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            
            // أضف ورقة عمل ثانية واضبط الصيغ التي تشير إلى Sheet1
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // اضبط الصيغ في Sheet1
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // أنشئ خيارات الإدراج مع تمكين UpdateReference
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // تتبع تغييرات الصيغ
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // أدرج صفوفًا ستقوم بتحديث الإشارات في الصيغ
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // أخرج عدد الخلايا التي تم تغييرها
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // اعرض الصيغ المحدثة
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### انظر أيضًا

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


