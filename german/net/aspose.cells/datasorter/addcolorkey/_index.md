---
title: "DataSorter.AddColorKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter-Methode. Fügt Farbsortierschlüssel hinzu"
type: docs
url: /de/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Fügt Farbsortierschlüssel hinzu.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | Int32 | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| Typ | SortOnType | Der Typ des sortierten Farbwerts. |
| Reihenfolge | SortOrder | Die Sortierreihenfolge. |
| Farbe | Farbe | Die benutzerdefinierte Sortierfarbe. |

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit farbigen Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // Wende Farben auf Zellen an
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // Daten‑Sortierer erstellen und Farbschlüssel hinzufügen
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // Daten sortieren
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // Die sortierten Werte ausgeben (zur Demonstration)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### Siehe auch

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


