---
title: "Cells.GetColumnWidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die Breite der angegebenen Spalte in der Normalansicht in Pixeln zurück"
type: docs
url: /de/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Pixel.

```csharp
public int GetColumnWidthPixel(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex |

### Rückgabewert

Breite der Spalte in der Normalansicht.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Spaltenbreite in Zeichen festlegen (wird in Pixel umgerechnet)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // Spaltenbreite in Pixeln abrufen
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // Gib das Ergebnis aus
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Pixel.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex |
| original | Boolean | Gibt an, ob die ursprüngliche Breite zurückgegeben wird, selbst wenn die Spalte ausgeblendet ist |

### Rückgabewert

Breite der Spalte in der Normalansicht.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Standardspaltenbreite auf 80 Pixel setzen
            worksheet.Cells.StandardWidthPixels = 80;

            // Spezifische Spaltenbreite für Spalte 2 (dritte Spalte) auf 120 Pixel setzen
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Aktuelle Breite mit Benutzeränderungen abrufen (original: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Ursprüngliche Breite ohne Änderungen abrufen (original: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Arbeitsmappe speichern, um die Persistenz der Spaltenbreite zu demonstrieren
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


