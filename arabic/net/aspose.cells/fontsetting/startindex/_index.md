---
title: "FontSetting.StartIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSetting. تحصل على الفهرس الابتدائي للأحرف"
type: docs
url: /ar/net/aspose.cells/fontsetting/startindex/
---
## FontSetting.StartIndex property

يحصل على الفهرس الابتدائي للأحرف.

```csharp
public int StartIndex { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyStartIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            string htmlText = "Normal <b>Bold Text</b> <i>Italic Text</i>";
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = htmlText;

            FontSetting[] fontSettings = cell.GetCharacters();
            
            Console.WriteLine("Text in cell: " + cell.StringValue);
            Console.WriteLine("\nFont settings analysis:");
            
            foreach (FontSetting fs in fontSettings)
            {
                string segment = cell.StringValue.Substring(fs.StartIndex, fs.Length);
                Console.WriteLine($"Text: '{segment}'");
                Console.WriteLine($"Starts at: {fs.StartIndex}, Length: {fs.Length}");
                Console.WriteLine($"Font is bold: {fs.Font.IsBold}");
                Console.WriteLine($"Font is italic: {fs.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


