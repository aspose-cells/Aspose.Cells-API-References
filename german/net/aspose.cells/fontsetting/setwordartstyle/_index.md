---
title: "FontSetting.SetWordArtStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSetting-Methode. Legt den voreingestellten WordArt-Stil fest"
type: docs
url: /de/net/aspose.cells/fontsetting/setwordartstyle/
---
## FontSetting.SetWordArtStyle method

Setzt den voreingestellten WordArt-Stil.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | PresetWordArtStyle | Der voreingestellte WordArt-Stil. |

### Hinweise

Nur für den Text von Form/Diagramm.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FontSettingMethodSetWordArtStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge etwas Text zu Zelle A1 hinzu
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text for WordArt");

            // Erstellen Sie eine Schriftarteinstellung für den Text in Zelle A1
            FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);

            try
            {
                // Wenden Sie den WordArt-Stil auf die Schriftarteinstellung an
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);

                Console.WriteLine("WordArt style applied successfully to the text.");
                
                // Zeigen Sie den Effekt, indem Sie die Arbeitsmappe speichern
                worksheet.AutoFitColumn(0);
                worksheet.AutoFitRow(0);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


