---
title: "PageSetup.SetHeaderPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تُعيّن صورة في رأس ورقة العمل"
type: docs
url: /ar/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

يضبط صورة في ترويسة ورقة العمل.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| headerPicture | Byte[] | بيانات الصورة. |

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

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تحميل ملف صورة إلى مصفوفة بايت
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // استدعِ SetHeaderPicture مع فهرس القسم (0 للرأس المركزي) وبيانات الصورة
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // تعيين نص الرأس لعرض الصورة
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


