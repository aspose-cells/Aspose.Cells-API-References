---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ErrorCheckOption. تحصل على عدد النطاقات التي تأثرت بهذا الإعداد"
type: docs
url: /ar/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

يحصل على عدد النطاقات المتأثرة بهذا الإعداد.

```csharp
public int GetCountOfRange()
```

### قيمة الإرجاع

عدد النطاقات التي تأثرت بهذا الإعداد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // احصل على مجموعة خيارات فحص الأخطاء
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // إضافة خيار فحص الأخطاء الأول
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // إضافة خيار فحص الأخطاء الثاني
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // عرض طريقة GetCountOfRange
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // احفظ المصنف
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


