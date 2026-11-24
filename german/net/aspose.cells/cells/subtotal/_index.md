---
title: "Cells.Subtotal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Erstellt Zwischensummen für den Bereich"
type: docs
url: /de/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Erstellt Zwischensummen für den Bereich.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der Bereich |
| groupBy | Int32 | Das Feld, nach dem gruppiert wird, als nullbasierter ganzzahliger Offset. |
| Funktion | ConsolidationFunction | Die Zwischensummen‑Funktion. |
| totalList | Int32[] | Ein Array von nullbasierten Feld‑Offsets, das die Felder angibt, zu denen die Zwischensummen hinzugefügt werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Zwischensummen füllen
            CreateSampleData(worksheet);

            // Definieren Sie den Zellbereich, der Daten enthält (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // Rufen Sie die Subtotal-Methode mit Parametern auf:
                // - Gruppieren nach Spalte 0 (Region)
                // - Verwenden Sie die SUM-Funktion
                // - Anwenden auf Spalte 2 (Verkäufe)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // Die Methoden ExpandColumnLevel und ExpandRowLevel wurden entfernt, um Kompilierungsfehler zu beheben
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Kopfzeilenzeile erstellen
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // Datenzeilen erstellen
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // Daten ab Zeile 2 (nullbasierter Index 1) füllen
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Erstellt Zwischensummen für den Bereich.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der Bereich |
| groupBy | Int32 | Das Feld, nach dem gruppiert wird, als nullbasierter ganzzahliger Offset. |
| Funktion | ConsolidationFunction | Die Zwischensummen‑Funktion. |
| totalList | Int32[] | Ein Array von nullbasierten Feld‑Offsets, das die Felder angibt, zu denen die Zwischensummen hinzugefügt werden. |
| replace | Boolean | Gibt an, ob die aktuellen Zwischensummen ersetzt werden sollen |
| pageBreaks | Boolean | Gibt an, ob zwischen Gruppen ein Seitenumbruch eingefügt werden soll |
| summaryBelowData | Boolean | Gibt an, ob eine Zusammenfassung unter den Daten hinzugefügt wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten für Zwischensummen erstellen
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // Definieren Sie den Zellbereich für Zwischensummen (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // Rufen Sie Subtotal mit Parametern auf:
                // - Gruppieren nach erster Spalte (0-basierter Index 0)
                // - Verwenden Sie die Sum-Funktion
                // - Auf die dritte Spalte anwenden (0-basierter Index 2)
                // - Vorhandene Zwischensummen ersetzen, Seitenumbrüche zwischen Gruppen, Zusammenfassung unter den Daten
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


