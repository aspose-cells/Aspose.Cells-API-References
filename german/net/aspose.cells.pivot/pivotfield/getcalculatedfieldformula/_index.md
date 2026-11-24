---
title: "PivotField.GetCalculatedFieldFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Gibt die Formelzeichenfolge des angegebenen berechneten Feldes zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/getcalculatedfieldformula/
---
## PivotField.GetCalculatedFieldFormula method

Gibt die Formelzeichenfolge des angegebenen berechneten Feldes zurück.

```csharp
[Obsolete("Use PivotField.GetFormula() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string GetCalculatedFieldFormula()
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotField.GetFormula(). Diese Methode wird 12 Monate später, seit August 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetCalculatedFieldFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["C1"].Value = "Profit";
            worksheet.Cells["C2"].Value = 20;
            worksheet.Cells["C3"].Value = 30;
            worksheet.Cells["C4"].Value = 25;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Profit");

            // Fügen Sie ein berechnetes Feld mit der PivotFieldCollection hinzu
            PivotFieldCollection pivotFields = pivotTable.DataFields;
            pivotTable.AddCalculatedField("ProfitMargin", "Profit/Sales", true);

            try
            {
                // Holen Sie das berechnete Feld aus DataFields
                PivotField calculatedField = pivotTable.DataFields[2]; // Index 2 for the calculated field

                // Prüfen Sie, ob es ein berechnetes Feld ist
                if (calculatedField.IsCalculatedField)
                {
                    // Holen Sie die Formel des berechneten Feldes
                    string formula = calculatedField.GetFormula();
                    Console.WriteLine($"Calculated field formula: {formula}");

                    // Speichere die Arbeitsmappe
                    workbook.Save("GetCalculatedFieldFormulaDemo.xlsx");
                    Console.WriteLine("Workbook saved successfully.");
                }
                else
                {
                    Console.WriteLine("The field is not a calculated field.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


