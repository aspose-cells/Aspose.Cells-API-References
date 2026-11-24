---
title: "Cells.DeleteBlankColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Lösche alle leeren Spalten, die keine Daten enthalten"
type: docs
url: /de/net/aspose.cells/cells/deleteblankcolumns/
---
## DeleteBlankColumns() {#deleteblankcolumns}

Löscht alle leeren Spalten, die keine Daten enthalten.

```csharp
public void DeleteBlankColumns()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Testdaten mit leeren Spalten hinzu
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B will be blank
            worksheet.Cells["A2"].PutValue("Data A");
            worksheet.Cells["C2"].PutValue("Data C");
            
            // Leere Spalten löschen
            worksheet.Cells.DeleteBlankColumns();
            
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

## DeleteBlankColumns(DeleteOptions) {#deleteblankcolumns_1}

Löscht alle leeren Spalten, die keine Daten enthalten.

```csharp
public void DeleteBlankColumns(DeleteOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | DeleteOptions | Die Optionen zum Löschen des Bereichs. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankColumnsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Daten mit leeren Spalten hinzu
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["C1"].PutValue("Column C"); // Column B is blank
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["C2"].PutValue(3);

            Console.WriteLine("Before deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 2 (0-based, column C)

            // Löschen-Optionen einrichten
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;

            // Leere Spalten löschen
            worksheet.Cells.DeleteBlankColumns(options);

            Console.WriteLine("After deleting blank columns:");
            Console.WriteLine($"MaxDataColumn: {worksheet.Cells.MaxDataColumn}"); // Should be 1 (0-based, column A and C remain, B was deleted)

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


