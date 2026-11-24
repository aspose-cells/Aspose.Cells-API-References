---
title: "PivotTable.RemoveField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Entfernt ein Feld aus einem bestimmten Feldbereich"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Entfernt ein Feld aus einem bestimmten Feldbereich

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | PivotFieldType | Der Feldbereichstyp. |
| fieldName | String | Der Name in den Basisfeldern. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Entferne Feld "c" aus dem Datenbereich
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // PivotTable-Daten berechnen
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Entfernt ein Feld aus einem bestimmten Pivot-Bereich.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | PivotFieldType | Der Feldbereichstyp. |
| baseFieldIndex | Int32 | Der Feldindex in den Basisfeldern. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Entferne das Zeilenfeld (Index 0) aus der Pivot-Tabelle
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Entferne Feld aus einem bestimmten Feldbereich

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | PivotFieldType | der Feldbereichstyp. |
| pivotField | PivotField | das Feld in den Basisfeldern. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Entferne ein Spaltenfeld aus der Pivot-Tabelle
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // Entferne ein Datenfeld aus der Pivot-Tabelle
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


