---
title: "Worksheet.AutoFitColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Passt die Spaltenbreite automatisch an"
type: docs
url: /de/net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

Passt die Spaltenbreite automatisch an.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |
| firstRow | Int32 | Index der ersten Zeile. |
| lastRow | Int32 | Index der letzten Zeile. |

### Hinweise

Diese Methode passt eine Zeile automatisch an den Inhalt eines Zellbereichs innerhalb der Zeile an.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zellen mit Beispieldaten füllen, die eine Anpassung der Spaltenbreite erfordern
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
            worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
            
            try
            {

                Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
                // Rufen Sie AutoFitColumn für Spalte A (Index 0) für die Zeilen 0 bis 2 (nullbasiert) auf
                worksheet.AutoFitColumn(0, 0, 2);
                
                Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
                
                // Zeigen Sie den Effekt, indem Sie die Spaltenbreite vor und nachher anzeigen
                Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

Passt die Spaltenbreite automatisch an.

```csharp
public void AutoFitColumn(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |

### Hinweise

AutoFitColumn ist eine ungenaue Funktion.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten zu Zellen in Spalte 4 (nullbasierter Index) hinzu
            worksheet.Cells["D1"].PutValue("This is a test");
            worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
            worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
            
            // Spalte 4 automatisch anpassen (nullbasierter Index)
            worksheet.AutoFitColumn(3);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


