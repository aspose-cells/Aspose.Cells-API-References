---
title: "Cells.GetRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt das Row-Element am angegebenen Zellenzeilenindex zurück"
type: docs
url: /de/net/aspose.cells/cells/getrow/
---
## Cells.GetRow method

Ruft das [`Row`](../../row/)‑Element am angegebenen Zellenzeilenindex ab.

```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |

### Rückgabewert

Falls das Zeilenobjekt existiert, gib das Row-Objekt zurück, andernfalls gib null zurück.

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Cells.CheckRow(int row)-Methode. Diese Methode wird 12 Monate später, seit Februar 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Zellen in Zeile 5, um sicherzustellen, dass die Zeile existiert
            worksheet.Cells["A5"].PutValue("Row 5 Data");
            worksheet.Cells["B5"].PutValue(12345);

            try
            {
                // Rufe die GetRow-Methode mit einem Int32-Parameter auf
                Row resultRow = worksheet.Cells.GetRow(5);

                if (resultRow != null)
                {
                    // Demonstriere Zeilenmanipulation
                    resultRow.Height = 20;
                    Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
                    
                    // Zähle Zellen in der Zeile
                    int cellCount = 0;
                    foreach (Cell cell in resultRow)
                    {
                        cellCount++;
                    }
                    Console.WriteLine($"Row 5 contains {cellCount} cells");
                }
                else
                {
                    Console.WriteLine("Row 5 not found in worksheet");
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid row index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRow: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


