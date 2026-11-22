---
title: "PageSetup.SetFooterPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. تعيين صورة في تذييل ورقة العمل"
type: docs
url: /ar/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

يضبط صورة في تذييل ورقة العمل.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |
| footerPicture | Byte[] | بيانات الصورة. |

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

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تحميل ملف صورة إلى مصفوفة بايت
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // استدعاء طريقة SetFooterPicture مع فهرس القسم (0 للوسط، 1 لليسار، 2 لليمين) وبيانات الصورة
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // تعيين نص التذييل للعرض مع الصورة
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // احفظ المصنف لرؤية صورة التذييل
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
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


