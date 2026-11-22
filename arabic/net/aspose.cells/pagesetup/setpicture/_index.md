---
title: "PageSetup.SetPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تقوم بتعيين صورة في رأس/تذييل ورقة العمل"
type: docs
url: /ar/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

يضبط صورة في الترويسة/التذييل لورقة العمل.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isFirst | منطقي | يشير إلى ما إذا كان يتم تعيين صورة رأس/تذييل الصفحة الأولى |
| isEven | منطقي | يشير إلى ما إذا كان يتم تعيين صورة رأس/تذييل الصفحة الزوجية |
| isHeader | منطقي | يشير إلى ما إذا كان يتم تعيين صورة رأس/تذييل |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| imageData | Byte[] | بيانات الصورة. |

### قيمة الإرجاع

يعيد [`Picture`](../../../aspose.cells.drawing/picture/) كائن.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // تحميل ملف صورة إلى مصفوفة بايت
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // استدعِ طريقة SetPicture لتعيين صورة الرأس
                // المعلمات: isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // تعيين نص الرأس
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // احفظ المصنف
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


