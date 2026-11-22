---
title: "Cell.GetCharacters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تُرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية.

```csharp
public FontSetting[] GetCharacters()
```

### قيمة الإرجاع

جميع كائنات Characters

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين نص منسق بـ HTML في الخلية A1 بأجزاء تنسيق مختلفة
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // الحصول على معلومات تنسيق الأحرف من الخلية A1
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // إخراج معلومات التنسيق
            Console.WriteLine("Character formatting in cell A1:");
            for (int i = 0; i < fontSettings.Length; i++)
            {
                Console.WriteLine($"Part {i + 1}:");
                Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
                Console.WriteLine($"Length: {fontSettings[i].Length}");
                Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
                Console.WriteLine();
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| علامة | منطقي | يشير إلى ما إذا كان تطبيق نمط الجدول على الخلية عندما تكون الخلية داخل جدول. |

### قيمة الإرجاع

جميع كائنات Characters

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة نص إلى الخلية C8 مع التنسيق
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // تنسيق أجزاء من النص
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // احصل على جميع إعدادات الخط مع التنسيق
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // عرض ألوان الخط
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


