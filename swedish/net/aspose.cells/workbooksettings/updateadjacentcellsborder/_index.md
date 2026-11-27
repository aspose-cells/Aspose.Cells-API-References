---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Anger om gränsen för intilliggande celler ska uppdateras"
type: docs
url: /sv/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Anger om gränsen för intilliggande celler ska uppdateras.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Anmärkningar

Standardvärdet är falskt. Till exempel: den nedre kanten på cell A1 uppdateras, den övre kanten på cell A2 bör också ändras.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Aktivera uppdatering av intilliggande cellers kanter
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange värde och applicera kant på cell A1
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // Ange värde till intilliggande cell B1 (höger om A1)
            worksheet.Cells["B1"].PutValue("Adjacent");

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


