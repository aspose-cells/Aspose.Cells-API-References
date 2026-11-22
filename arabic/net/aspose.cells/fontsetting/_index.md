---
title: "الفئة FontSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.FontSetting. تمثل نطاقًا من الأحرف داخل نص الخلية"
type: docs
url: /ar/net/aspose.cells/fontsetting/
---
## FontSetting class

يمثل نطاقًا من الأحرف داخل نص الخلية.

```csharp
public class FontSetting
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | يعيد الخط لهذا الكائن. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | يحصل على طول الأحرف. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | يحصل على الفهرس الابتدائي للأحرف. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | يعيد خيارات النص. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | يحصل على نوع عقدة النص. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | يضبط نمط WordArt المسبق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى كائن Excel
            workbook.Worksheets.Add();

            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية "A1" من ورقة العمل
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // إضافة قيمة إلى الخلية "A1"
            cell.PutValue("Visit Aspose!");

            // الحصول على نطاق الأحرف
            FontSetting character = cell.Characters(6, 7);

            // ضبط خط الأحرف المحددة إلى غامق
            character.Font.IsBold = true;

            // ضبط لون خط الأحرف المحددة إلى أزرق
            character.Font.Color = Color.Blue;

            // حفظ ملف Excel
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


