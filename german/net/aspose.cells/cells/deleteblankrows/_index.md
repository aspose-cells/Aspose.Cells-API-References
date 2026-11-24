---
title: "Cells.DeleteBlankRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells‑Methode. Löscht alle leeren Zeilen, die keine Daten oder andere Objekte enthalten"
type: docs
url: /de/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Lösche alle leeren Zeilen, die keine Daten oder andere Objekte enthalten.

```csharp
public void DeleteBlankRows()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie einige Daten mit leeren Zeilen hinzu
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Leere Zeilen löschen
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Lösche alle leeren Zeilen, die keine Daten oder einige spezielle Objekte wie sichtbare Kommentare und Pivot-Tabellen enthalten.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | DeleteOptions | Die Optionen zum Löschen des Bereichs. |

### Hinweise

Für leere Zeilen, die gelöscht werden sollen, ist es nicht nur erforderlich, dass [`IsBlank`](../../row/isblank/) wahr ist, sondern es darf auch kein sichtbarer Kommentar für irgendeine Zelle in diesen Zeilen definiert sein und es darf keine Pivot‑Tabelle geben, deren Bereich mit ihnen überschneidet.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Testdaten mit leeren Zeilen hinzu
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // Löschoptionen erstellen
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // Leere Zeilen löschen
            sheet.Cells.DeleteBlankRows(options);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


