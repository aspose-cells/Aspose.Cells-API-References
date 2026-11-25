---
title: "PivotField.FilterByValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Filtra per valori del campo pivot dei dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/filterbyvalue/
---
## PivotField.FilterByValue method

Filtra per valori del campo pivot dei dati.

```csharp
public PivotFilter FilterByValue(int valueFieldIndex, PivotFilterType type, double value1, 
    double value2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valueFieldIndex | Int32 | L'indice del campo valore nella regione dei valori. |
| type | PivotFilterType | Il tipo di dati di filtraggio. |
| value1 | Double | Il valore della condizione di filtro |
| value2 | Double | Il valore superiore della condizione di filtro tra |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodFilterByValueWithInt32PivotFilterTypeDoubleDoubDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["B3"].Value = 1.8;
            worksheet.Cells["B4"].Value = 3.2;
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["C2"].Value = 100;
            worksheet.Cells["C3"].Value = 150;
            worksheet.Cells["C4"].Value = 80;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campi dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Chiama il metodo FilterByValue con i parametri (Int32, PivotFilterType, Double, Double)
                // Filtra i prodotti dove Quantità (indice campo 1) è compresa tra 90 e 160
                PivotFilter filter = pivotField.FilterByValue(1, PivotFilterType.ValueBetween, 90.0, 160.0);

                Console.WriteLine("FilterByValue method executed successfully");
                Console.WriteLine($"Filter type: {filter.FilterType}");
                Console.WriteLine($"Value field index: {filter.ValueFieldIndex}");

                // Aggiorna la tabella pivot per mostrare le modifiche
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FilterByValue method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("PivotFieldMethodFilterByValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


