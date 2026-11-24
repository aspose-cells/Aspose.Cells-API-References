---
title: "PivotTable.GetFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Gibt die spezifische Pivot-Feldliste für die Region zurück."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/getfields/
---
## PivotTable.GetFields method

Ruft die spezifische PivotField‑Liste nach Region ab.

```csharp
public PivotFieldCollection GetFields(PivotFieldType fieldType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | PivotFieldType | der Regionstyp. |

### Rückgabewert

die spezifische Pivot-Feldsammlung

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodGetFieldsWithPivotFieldTypeDemo
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
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Rufen Sie die GetFields-Methode mit dem Parameter PivotFieldType.Row auf.
                PivotFieldCollection rowFields = pivotTable.GetFields(PivotFieldType.Row);
                
                Console.WriteLine($"Number of row fields: {rowFields.Count}");
                foreach (PivotField field in rowFields)
                {
                    Console.WriteLine($"Row field name: {field.Name}");
                }

                // Rufen Sie die GetFields-Methode mit dem Parameter PivotFieldType.Data auf.
                PivotFieldCollection dataFields = pivotTable.GetFields(PivotFieldType.Data);
                
                Console.WriteLine($"Number of data fields: {dataFields.Count}");
                foreach (PivotField field in dataFields)
                {
                    Console.WriteLine($"Data field name: {field.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFields method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableGetFieldsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


