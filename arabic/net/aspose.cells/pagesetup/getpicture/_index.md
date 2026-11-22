---
title: "PageSetup.GetPicture"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PageSetup. يحصل على كائن Picture للترويسة / التذييل"
type: docs
url: /ar/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

يحصل على كائن [`Picture`](../../../aspose.cells.drawing/picture/) للترويسة / التذييل.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isHeader | منطقي | يشير إلى ما إذا كان في الترويسة أم التذييل. |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

### قيمة الإرجاع

يرجع كائن [`Picture`](../../../aspose.cells.drawing/picture/). يرجع null إذا لم توجد صورة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة صورة إلى ترويسة ورقة العمل
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // احصل على الصورة من الترويسة وعدل سطوعها
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

يحصل على كائن [`Picture`](../../../aspose.cells.drawing/picture/) للترويسة / التذييل.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isFirst | منطقي | يشير إلى ما إذا كان يتم الحصول على صورة ترويسة/تذييل الصفحة الأولى. |
| isEven | منطقي | يشير إلى ما إذا كان يتم الحصول على صورة ترويسة/تذييل الصفحات الزوجية. |
| isHeader | منطقي | يشير إلى ما إذا كان يتم الحصول على صورة الترويسة/التذييل. |
| قسم | Int32 | 0: القسم الأيسر، 1: القسم الأوسط، 2: القسم الأيمن. |

### قيمة الإرجاع

يعيد [`Picture`](../../../aspose.cells.drawing/picture/) كائن.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على كائن PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين بعض خصائص الترويسة/التذييل لضمان وجود صور يمكن استرجاعها
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // استدعِ طريقة GetPicture مع المعاملات: isFirst, isEven, isHeader, section
                // التحقق من رأس الصفحة الأولى (القسم 0 - رأس مركزي)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // احفظ المصنف
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
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


