---
title: "Cell.SetCharacters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تعيين تنسيق النص الغني للخلية"
type: docs
url: /ar/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

يضبط تنسيق النص الغني للخلية.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| حروف | FontSetting[] | جميع كائنات Characters. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellMethodSetCharactersWithFontSettingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // قم بتعيين قيمة الخلية لتطبيق تنسيق النص الغني
            cell.Value = "Hello World!";

            try
            {
                // إنشاء إعدادات الخط لأجزاء مختلفة من النص
                FontSetting[] fontSettings = new FontSetting[2];

                // تنسيق أول 5 أحرف (Hello) كخط غامق أحمر
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // تنسيق الأحرف المتبقية ( World!) كخط مائل أزرق
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // تطبيق إعدادات الأحرف المنسقة باستخدام SetCharacters
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


