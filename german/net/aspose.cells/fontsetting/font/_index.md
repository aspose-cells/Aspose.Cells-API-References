---
title: "FontSetting.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSetting Eigenschaft. Gibt die Schriftart dieses Objekts zurück"
type: docs
url: /de/net/aspose.cells/fontsetting/font/
---
## FontSetting.Font property

Gibt die Schriftart dieses Objekts zurück.

```csharp
public Font Font { get; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            cell.PutValue("Sample text for font formatting demonstration");
            
            // Wenden Sie verschiedene Schriftarteigenschaften auf Zeichenbereiche an
            cell.Characters(0, 6).Font.IsBold = true;
            cell.Characters(7, 4).Font.Color = Color.Blue;
            cell.Characters(12, 5).Font.IsItalic = true;
            cell.Characters(18, 10).Font.IsStrikeout = true;
            cell.Characters(29, 13).Font.Name = "Courier New";
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontSettingDemo.xlsx");
            
            // Überprüfen Sie die gespeicherte Datei
            Workbook verifyWorkbook = new Workbook("FontSettingDemo.xlsx");
            Cell verifyCell = verifyWorkbook.Worksheets[0].Cells["A1"];
            
            Console.WriteLine("Font formatting applied successfully:");
            foreach (FontSetting setting in verifyCell.GetCharacters())
            {
                Console.WriteLine($"Characters {setting.StartIndex}-{setting.StartIndex + setting.Length - 1}:");
                Console.WriteLine($"  Bold: {setting.Font.IsBold}");
                Console.WriteLine($"  Italic: {setting.Font.IsItalic}");
                Console.WriteLine($"  Strikeout: {setting.Font.IsStrikeout}");
                Console.WriteLine($"  Color: {setting.Font.Color}");
                Console.WriteLine($"  Font: {setting.Font.Name}");
            }
        }
    }
}
```

### Siehe auch

* class [Font](../../font/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


