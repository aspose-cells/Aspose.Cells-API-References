---
title: "MsoFillFormatHelper.BackColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormatHelper property. Hämtar och anger filens bakgrundsfärg"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Hämtar och anger filens bakgrundsfärg.

```csharp
public Color BackColor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en etikett bara för att ha lite innehåll i bladet
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper exponerar inte en publik konstruktor, använd reflektion för att skapa en instans av den
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Ange BackColor till en känd färg (t.ex. LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // Läs tillbaka BackColor‑värdet och visa det
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // Alternativt kan du också läsa ForeColor för att visa att den förblir standard
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Spara arbetsboken – fill‑hjälparen är inte kopplad till en form,
                // men sparandet visar att koden kördes utan fel.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


