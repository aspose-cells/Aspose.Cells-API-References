---
title: "التعداد MsoDrawingType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.MsoDrawingType. يمثل نوع كائنات الرسم المكتبية"
type: docs
url: /ar/net/aspose.cells.drawing/msodrawingtype/
---
## MsoDrawingType enumeration

يمثل نوع كائنات الرسم المكتبية.

```csharp
public enum MsoDrawingType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Group | `0` | مجموعة |
| Line | `1` | خط |
| Rectangle | `2` | مستطيل |
| Oval | `3` | بيضاوي |
| Arc | `4` | قوس |
| Chart | `5` | مخطط |
| TextBox | `6` | مربع نص |
| Button | `7` | زر |
| Picture | `8` | صورة |
| Polygon | `9` | مضلع |
| CheckBox | `11` | مربع اختيار |
| RadioButton | `12` | زر راديو |
| Label | `14` | تسمية |
| DialogBox | `15` | مربع حوار |
| Spinner | `16` | دوار |
| ScrollBar | `17` | شريط تمرير |
| ListBox | `18` | مربع قائمة |
| GroupBox | `19` | مربع مجموعة |
| ComboBox | `20` | قائمة منسدلة |
| Comment | `25` | تعليق |
| OleObject | `24` | OleObject |
| CellsDrawing | `30` | فقط للحفاظ على كائن الرسم في ملف القالب. |
| Unknown | `29` | فقط للحفاظ على كائن الرسم في ملف xlsx. |
| Slicer | `31` | مقسم |
| WebExtension | `32` | ملحق ويب |
| SmartArt | `33` | فن ذكي |
| CustomXml | `34` | شكل XML مخصص، مثل الحبر. |
| Timeline | `35` | خط زمني |
| Model3D | `36` | نموذج ثلاثي الأبعاد |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoDrawingTypeDemo
    {
        public static void MsoDrawingTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلًا إلى ورقة العمل
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            rectangle.Name = "MyRectangle";
            rectangle.AlternativeText = "This is a rectangle shape";

            // أضف شكلاً بيضاويًا إلى ورقة العمل
            Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
            oval.Name = "MyOval";
            oval.AlternativeText = "This is an oval shape";

            // أضف شكل خط إلى ورقة العمل
            Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
            line.Name = "MyLine";
            line.AlternativeText = "This is a line shape";

            // أضف شكل مربع نص إلى ورقة العمل
            Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
            textBox.Name = "MyTextBox";
            textBox.AlternativeText = "This is a textbox shape";
            textBox.Text = "Hello, Aspose.Cells!";

            // أخرج أسماء الأنواع للأشكال
            foreach (Shape shape in worksheet.Shapes)
            {
                Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
            }

            // احفظ المصنف
            workbook.Save("MsoDrawingTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


