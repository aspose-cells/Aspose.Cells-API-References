---
title: "Cells.DeleteColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht mehrere Spalten"
type: docs
url: /de/net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Löscht mehrere Spalten.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Index der ersten zu löschenden Spalte. |
| totalColumns | Int32 | Anzahl der zu löschenden Spalten. |
| updateReference | Boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Füge eine Formel hinzu, die diese Spalten referenziert
            worksheet.Cells["D1"].Formula = "=SUM(A2:C2)";

            Console.WriteLine("Before deleting columns:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1: " + worksheet.Cells["C1"].Value);
            Console.WriteLine("D1 formula: " + worksheet.Cells["D1"].Formula);

            // Lösche Spalte B (Index 1) und verschiebe die verbleibenden Spalten nach links
            worksheet.Cells.DeleteColumns(1, 1, true);

            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1 formula: " + worksheet.Cells["C1"].Formula);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Löscht mehrere Spalten.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Index der ersten zu löschenden Spalte. |
| totalColumns | Int32 | Anzahl der zu löschenden Spalten. |
| Optionen | DeleteOptions | Optionen für den Löschvorgang |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fülle Beispieldaten in den Spalten A-E
            for (int col = 0; col < 5; col++)
            {
                worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
                worksheet.Cells[1, col].Value = $"Data{col + 1}";
            }

            // Erstelle DeleteOptions und konfiguriere die Einstellungen
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Update references in other cells
            };

            try
            {
                // Lösche 2 Spalten, beginnend mit Spalte B (Index 1)
                worksheet.Cells.DeleteColumns(1, 2, options);
                
                Console.WriteLine("Deleted columns B and C successfully");
                
                // Zeige die verbleibenden Daten in Spalte B (ursprüngliche Spalte D)
                Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
            }
            
            // Speichere die geänderte Arbeitsmappe
            workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


