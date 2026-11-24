---
title: "Cells.CopyRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Kopiert Daten und Formate einiger ganzer Zeilen"
type: docs
url: /de/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Kopiert Daten und Formate einiger ganzer Zeilen.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceRowIndex | Int32 | Quell‑Zeilenindex. |
| destinationRowIndex | Int32 | Zielzeilenindex. |
| rowNumber | Int32 | Die kopierte Zeilennummer. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // Füge dem Quellarbeitsbuch einige Beispieldaten hinzu
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // Hole die Zellen aus beiden Arbeitsbüchern
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // Kopiere alle Zeilen von der Quelle zum Ziel, beginnend bei Zeile 0 im Ziel
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // Ergebnis speichern
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Kopiert Daten und Formate einiger ganzer Zeilen.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceRowIndex | Int32 | Quell‑Zeilenindex. |
| destinationRowIndex | Int32 | Zielzeilenindex. |
| rowNumber | Int32 | Die kopierte Zeilennummer. |
| copyOptions | CopyOptions | Die Kopieroptionen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten und Hyperlinks hinzu
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Füge eine leere Zeile bei Zeile 5 ein
            worksheet.Cells.InsertRows(5, 1);

            // Kopiere Zeile 4 nach Zeile 5 ohne CopyOptions
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // Setze das Arbeitsblatt zurück
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Füge erneut eine leere Zeile bei Zeile 5 ein
            worksheet.Cells.InsertRows(5, 1);

            // Kopiere Zeile 4 nach Zeile 5 mit CopyOptions
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Kopiert Daten und Formate einiger ganzer Zeilen.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceCells0 | Zellen | Quell‑Cells‑Objekt enthält zu kopierende Daten und Formate. |
| sourceRowIndex | Int32 | Quell‑Zeilenindex. |
| destinationRowIndex | Int32 | Zielzeilenindex. |
| rowNumber | Int32 | Die kopierte Zeilennummer. |
| copyOptions | CopyOptions | Die Kopieroptionen. |
| pasteOptions | PasteOptions | Die Optionen für das Einfügen. |

### Siehe auch

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


