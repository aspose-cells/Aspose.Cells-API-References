---
title: "Cell.NumberCategoryType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تمثل نوع الفئة لتنسيق الأرقام في هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

يمثل نوع الفئة لتنسيق الأرقام في هذه الخلية.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### ملاحظات

عندما يتم دمج نمط تنسيق الخلية مع أنماط التنسيق الشرطي، يكون النوع المرجع مطابقًا للجزء المستخدم للقيمة الحالية لهذه الخلية. على سبيل المثال، إذا كان نمط التنسيق لهذه الخلية هو "#,##0;(#,##0);"-";@"، فإن عندما تكون قيمة الخلية رقمية وغير صفرية، يكون النوع المرجع هو Number؛ عندما تكون قيمة الخلية صفرًا أو ليست قيمة رقمية، يكون النوع المرجع هو Text.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف قيمة تاريخ إلى الخلية A1
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // حدد تنسيق التاريخ
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // أضف قيمة رقمية إلى الخلية A2
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // أضف قيمة نصية إلى الخلية A3
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // عرض NumberCategoryType لكل خلية
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // غيّر الخلية A2 إلى تنسيق العملة وتحقق من NumberCategoryType
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### انظر أيضًا

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


