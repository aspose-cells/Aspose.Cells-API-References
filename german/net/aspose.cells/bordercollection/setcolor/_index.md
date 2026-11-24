---
title: "BorderCollection.SetColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BorderCollection‑Methode. Setzt die Farbe aller Rahmen in der Sammlung"
type: docs
url: /de/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Setzt die Farbe aller Rahmen in der Sammlung.

```csharp
public void SetColor(Color color)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbe | Farbe | Farbe der Rahmen. |

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Stil mit farbigen Rahmen
            Style style = workbook.CreateStyle();
            
            // Setze Rahmenlinienstile
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Setze die Rahmenfarbe auf Rot mittels SetColor‑Methode
            style.Borders.SetColor(Color.Red);

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // Spalte automatisch anpassen für bessere Sichtbarkeit
            worksheet.AutoFitColumn(0);

            // Speichere die Arbeitsmappe
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


