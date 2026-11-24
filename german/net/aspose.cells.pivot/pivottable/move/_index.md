---
title: "PivotTable.Move"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable method. Verschiebt die PivotTable an einen anderen Ort im Arbeitsblatt"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/move/
---
## Move(int, int) {#move}

Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| column | Int32 | Spaltenindex. |

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.MoveTo(). Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Daten berechnen, um die Pivot-Tabelle zu füllen
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table created at E3");

            try
            {
                // Verschieben Sie die Pivot‑Tabelle an einen neuen Ort (Zeile 10, Spalte 5)
                pivotTable.Move(10, 5);
                Console.WriteLine("Pivot table moved to row 10, column 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableMethodMoveWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(string) {#move_1}

Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(string destCellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destCellName | String | der Zielzellenname. |

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotTable.MoveTo(). Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Verschieben Sie die Pivot‑Tabelle an einen neuen Ort mithilfe des Zellnamens
                pivotTable.Move("G10");

                Console.WriteLine("PivotTable moved successfully to G10");
                Console.WriteLine($"New location: {pivotTable.TableRange1.StartRow}, {pivotTable.TableRange1.StartColumn}");

                // Speichere die Arbeitsmappe
                workbook.Save("PivotTableMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error moving PivotTable: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


