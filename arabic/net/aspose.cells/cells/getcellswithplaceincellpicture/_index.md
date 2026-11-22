---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على جميع الخلايا التي تحتوي على صورة مدمجة"
type: docs
url: /ar/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

يحصل على جميع الخلايا التي تحتوي على صورة مدمجة.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### قيمة الإرجاع

المُعدد لتعداد جميع كائنات Cell التي تحتوي على صورة مدمجة

### ملاحظات

إذا لم توجد صورة تم تعيينها كـ "Place in Cell" في هذه ورقة العمل، سيتم إرجاع null.

### أمثلة

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // أضف صورة إلى ورقة العمل (لن يتم احتسابها بواسطة GetCellsWithPlaceInCellPicture)
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // أضف صورة مدمجة إلى الخلية B3 (سيتم احتسابها)
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // إزالة الصورة العائمة
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // احصل على الخلايا التي تحتوي على صور مدمجة
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // احفظ وأعد التحميل للتحقق من الاستمرارية
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // تحقق بعد إعادة التحميل
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


