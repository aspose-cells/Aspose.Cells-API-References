---
title: "FontSetting.StartIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSetting-egenskap. Hämtar startindex för tecknen"
type: docs
url: /sv/net/aspose.cells/fontsetting/startindex/
---
## FontSetting.StartIndex property

Hämtar startindexet för tecknen.

```csharp
public int StartIndex { get; }
```

### Exempel

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

### Se även

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


