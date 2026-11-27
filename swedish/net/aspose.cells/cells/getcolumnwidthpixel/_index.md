---
title: "Cells.GetColumnWidthPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar bredden på den angivna kolumnen i normal vy i enheter av pixel"
type: docs
url: /sv/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Hämtar bredden för den angivna kolumnen i normal vy, i pixlar.

```csharp
public int GetColumnWidthPixel(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex |

### Returvärde

Kolumnens bredd i normal vy.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in kolumnbredd i tecken (kommer att konverteras till pixlar)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // Hämta kolumnbredd i pixlar
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // Skriv ut resultatet
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Hämtar bredden för den angivna kolumnen i normal vy, i pixlar.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex |
| original | Boolean | Indikerar om den ursprungliga bredden returneras även när kolumnen är dold |

### Returvärde

Kolumnens bredd i normal vy.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället Cells.GetColumnWidth(int ,bool , CellsUnitType )-metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in standardkolumnbredd till 80 pixlar
            worksheet.Cells.StandardWidthPixels = 80;

            // Ställ in specifik kolumnbredd för kolumn 2 (tredje kolumnen) till 120 pixlar
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Hämta aktuell bredd med användarmodifikationer (original: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Hämta originalbredd utan modifikationer (original: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Spara arbetsboken för att demonstrera kolumnbreddens beständighet
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


