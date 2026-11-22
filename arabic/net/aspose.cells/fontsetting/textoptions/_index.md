---
title: "FontSetting.TextOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSetting. تُرجع خيارات النص"
type: docs
url: /ar/net/aspose.cells/fontsetting/textoptions/
---
## FontSetting.TextOptions property

يعيد خيارات النص.

```csharp
public TextOptions TextOptions { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyTextOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نص تجريبي مع أقسام تنسيق مختلفة
            string part1 = "This is normal text. ";
            string part2 = "This is bold and italic text. ";
            string part3 = "This is normal again. ";
            string part4 = "This is bold text.";
            
            // دمج جميع الأجزاء في خلية واحدة
            Cell cell = worksheet.Cells["A1"];
            cell.Value = part1 + part2 + part3 + part4;
            
            // تطبيق التنسيق على أجزاء محددة من النص
            int startPos1 = part1.Length;
            int length1 = part2.Length;
            cell.Characters(startPos1, length1).TextOptions.IsBold = true;
            cell.Characters(startPos1, length1).TextOptions.IsItalic = true;
            
            int startPos2 = part1.Length + part2.Length + part3.Length;
            int length2 = part4.Length;
            cell.Characters(startPos2, length2).TextOptions.IsBold = true;
            
            // احفظ المصنف
            workbook.Save("TextOptionsDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("TextOptions demo completed. File saved.");
        }
    }
}
```

### انظر أيضًا

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


