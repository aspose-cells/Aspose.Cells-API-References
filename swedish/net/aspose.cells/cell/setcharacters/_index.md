---
title: "Cell.SetCharacters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Ställer in rik textformat för cellen"
type: docs
url: /sv/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

Ställer in rik textformat för cellen.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tecken | FontSetting[] | Alla teckenobjekt. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Ange cellvärde för att tillämpa rik textformatering
            cell.Value = "Hello World!";

            try
            {
                // Skapa teckensnittinställningar för olika delar av texten
                FontSetting[] fontSettings = new FontSetting[2];

                // Formatera de första 5 tecknen (Hello) som fet röd
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // Formatera återstående tecken ( World!) som kursiv blå
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // Tillämpa de formaterade teckeninställningarna med SetCharacters
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


