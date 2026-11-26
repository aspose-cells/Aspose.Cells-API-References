---
title: "FontSetting.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSetting. Devuelve la fuente de este objeto"
type: docs
url: /es/net/aspose.cells/fontsetting/font/
---
## FontSetting.Font property

Devuelve la fuente de este objeto.

```csharp
public Font Font { get; }
```

### Ejemplos

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
            
            // Aplicar diferentes propiedades de fuente a rangos de caracteres
            cell.Characters(0, 6).Font.IsBold = true;
            cell.Characters(7, 4).Font.Color = Color.Blue;
            cell.Characters(12, 5).Font.IsItalic = true;
            cell.Characters(18, 10).Font.IsStrikeout = true;
            cell.Characters(29, 13).Font.Name = "Courier New";
            
            // Guarda el libro de trabajo
            workbook.Save("FontSettingDemo.xlsx");
            
            // Verifique el archivo guardado
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

### Ver también

* class [Font](../../font/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


