---
title: "Cells.CopyColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Kopiert Daten und Formate einer gesamten Spalte"
type: docs
url: /de/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Kopiert Daten und Formate einer ganzen Spalte.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceColumnIndex | Int32 | Index der Quellspalte. |
| destinationColumnIndex | Int32 | Zielspaltenindex. |
| columnNumber | Int32 | Die Nummer der kopierten Spalte. |
| pasteOptions | PasteOptions | Die Optionen für das Einfügen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Ein weiteres Arbeitsbuch als Ziel erstellen
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // Spalten nur mit Formatierung kopieren
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

Kopiert Daten und Formate mehrerer Spalten.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceColumnIndex | Int32 | Index der Quellspalte. |
| destinationColumnIndex | Int32 | Zielspaltenindex. |
| columnNumber | Int32 | Die Nummer der kopierten Spalte. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten zu Spalten hinzufügen
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // Spalten von Spaltenindex 1 (B) bis Spaltenindex 3 (D) kopieren, 1 Spalte kopieren
            cells.CopyColumns(cells, 1, 3, 1);

            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Kopiert Daten und Formate aller Spalten.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceColumnIndex | Int32 | Index der Quellspalte. |
| sourceTotalColumns | Int32 | Die Anzahl der Quellspalten. |
| destinationColumnIndex | Int32 | Zielspaltenindex. |
| destinationTotalColumns | Int32 | Die Anzahl der Zielspalten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Quellspalten füllen (Spalten 0 und 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // Kopiere 2 Spalten von Index 0 zum Zielindex 3 und füge 2 Spalten ein
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // Kopieren überprüfen, indem die Zielspalten (3 und 4) geprüft werden
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


