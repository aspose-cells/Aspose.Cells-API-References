---
title: "Cells.GetCellDisplayStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt den Anzeigestil der angegebenen Zelle zurück."
type: docs
url: /de/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Ermittelt den Anzeigestil der angegebenen Zelle.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der angegebenen Zelle |
| column | Int32 | Spalte der angegebenen Zelle |

### Rückgabewert

Der Anzeigestil der angegebenen Zelle.

### Hinweise

Das Gleiche gilt für [`GetDisplayStyle`](../../cell/getdisplaystyle/), und das Gleiche gilt beim Verwenden von SideBorders für `GetCellDisplayStyle`.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Zellstil für die Demonstration vorbereiten
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // Benutzerdefinierten Stil erstellen
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Stil auf Zelle anwenden
            cell.SetStyle(style);

            try
            {
                // Rufen Sie GetCellDisplayStyle mit Zeile 0 und Spalte 0 auf
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // Eigenschaften des Anzeigestils
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // Den Anzeigestil auf eine andere Zelle anwenden, um die visuelle Überprüfung durchzuführen
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Ermittelt den Anzeigestil der angegebenen Zelle.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex der angegebenen Zelle |
| column | Int32 | Spalte der angegebenen Zelle |
| adjacentBorders | BorderType | Gibt an, welche Rahmen überprüft und an die Rahmen benachbarter Zellen angepasst werden müssen. Bitte siehe die Beschreibung desselben Parameters von [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### Rückgabewert

Der Anzeigestil der angegebenen Zelle.

### Hinweise

Wenn die Zelle auch von anderen Einstellungen wie bedingter Formatierung, Listobjekten usw. betroffen ist, kann der Anzeigestil von [`GetCellStyle`](../getcellstyle/) abweichen. Und da diese Einstellungen auch auf leere (nicht vorhandene) Zellen angewendet werden können, vermeidet die Verwendung dieser Methode die Instanziierung dieser leeren Zellen, sodass die Leistung besser ist, als die Cell‑Instanz aus Cells zu holen und anschließend [`GetDisplayStyle`](../../cell/getdisplaystyle/) aufzurufen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf Zelle A1 zu und setzen Sie einen Rahmenstil
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // Rufen Sie GetCellDisplayStyle mit spezifischen Parametern auf (0,0 für A1, Typ TopBorder)
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // Überprüfen Sie, ob der abgerufene Stil unserer Rahmenfarbe entspricht
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // Demonstrieren Sie die Stil-Anwendung, indem Sie eine andere Zelle ändern
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


