---
title: "PivotField.GetSubtotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Indica se mostrare il subtotale specificato per questo campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/getsubtotals/
---
## PivotField.GetSubtotals method

Indica se mostrare il subtotale specificato per questo campo pivot.

```csharp
public bool GetSubtotals(PivotFieldSubtotalType subtotalType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Tipo di subtotale. |

### Valore di ritorno

Restituisce se mostra il subtotale specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGetSubtotalsWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["A4"].Value = "Electronics";
            worksheet.Cells["A5"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 500;
            worksheet.Cells["B4"].Value = 1200;
            worksheet.Cells["B5"].Value = 600;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Verifica se il subtotale Somma è abilitato
                bool hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is enabled: {hasSumSubtotal}");

                // Verifica se il subtotale Media è abilitato
                bool hasAvgSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal is enabled: {hasAvgSubtotal}");

                // Abilita il subtotale Somma
                pivotField.SetSubtotals(PivotFieldSubtotalType.Sum, true);

                // Verifica che il subtotale Somma sia ora abilitato
                hasSumSubtotal = pivotField.GetSubtotals(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"After setting, Sum subtotal is enabled: {hasSumSubtotal}");

                // Aggiorna la tabella pivot per mostrare le modifiche
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSubtotals method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("PivotFieldMethodGetSubtotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


