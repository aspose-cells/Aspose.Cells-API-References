---
title: "PivotField.GetCalculatedFieldFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Ottieni la stringa della formula del campo calcolato specificato"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/getcalculatedfieldformula/
---
## PivotField.GetCalculatedFieldFormula method

Ottieni la stringa della formula del campo calcolato specificato.

```csharp
[Obsolete("Use PivotField.GetFormula() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string GetCalculatedFieldFormula()
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.GetFormula(). Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
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

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Profit");

            // Aggiungi un campo calcolato utilizzando PivotFieldCollection
            PivotFieldCollection pivotFields = pivotTable.DataFields;
            pivotTable.AddCalculatedField("ProfitMargin", "Profit/Sales", true);

            try
            {
                // Ottieni il campo calcolato da DataFields
                PivotField calculatedField = pivotTable.DataFields[2]; // Index 2 for the calculated field

                // Verifica se è un campo calcolato
                if (calculatedField.IsCalculatedField)
                {
                    // Ottieni la formula del campo calcolato
                    string formula = calculatedField.GetFormula();
                    Console.WriteLine($"Calculated field formula: {formula}");

                    // Salva la cartella di lavoro
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

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


