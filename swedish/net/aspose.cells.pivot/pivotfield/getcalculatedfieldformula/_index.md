---
title: "PivotField.GetCalculatedFieldFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Hämta formelsträngen för det angivna beräknade fältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/getcalculatedfieldformula/
---
## PivotField.GetCalculatedFieldFormula method

Hämta formelsträngen för det angivna beräknade fältet.

```csharp
[Obsolete("Use PivotField.GetFormula() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string GetCalculatedFieldFormula()
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.GetFormula()-metoden. Denna metod kommer att tas bort 12 månader senare från och med augusti 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
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

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Profit");

            // Lägg till ett beräknat fält med hjälp av PivotFieldCollection
            PivotFieldCollection pivotFields = pivotTable.DataFields;
            pivotTable.AddCalculatedField("ProfitMargin", "Profit/Sales", true);

            try
            {
                // Hämta det beräknade fältet från DataFields
                PivotField calculatedField = pivotTable.DataFields[2]; // Index 2 for the calculated field

                // Kontrollera om det är ett beräknat fält
                if (calculatedField.IsCalculatedField)
                {
                    // Hämta formeln för det beräknade fältet
                    string formula = calculatedField.GetFormula();
                    Console.WriteLine($"Calculated field formula: {formula}");

                    // Spara arbetsboken
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

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


