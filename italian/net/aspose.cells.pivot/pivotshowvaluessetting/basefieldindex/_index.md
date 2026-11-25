---
title: "PivotShowValuesSetting.BaseFieldIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotShowValuesSetting. Rappresenta il campo base per un calcolo ShowDataAs quando il calcolo ShowDataAs è in uso"
type: docs
url: /it/net/aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/
---
## PivotShowValuesSetting.BaseFieldIndex property

Rappresenta il campo base per un calcolo ShowDataAs quando il calcolo ShowDataAs è in uso.

```csharp
public int BaseFieldIndex { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingPropertyBaseFieldIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            try
            {
                // Crea tabella pivot
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Aggiungi campi alla tabella pivot
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Ottieni il campo dati e la sua impostazione di visualizzazione dei valori
                PivotField dataField = pivotTable.DataFields[0];
                PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

                // Imposta il tipo di calcolo per dimostrare l'uso di BaseFieldIndex
                showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;

                // Imposta e ottieni la proprietà BaseFieldIndex
                showValuesSetting.BaseFieldIndex = 0;
                Console.WriteLine("BaseFieldIndex value: " + showValuesSetting.BaseFieldIndex);

                // Aggiorna e calcola la tabella pivot
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Salva la cartella di lavoro
                workbook.Save("BaseFieldIndexDemo.xlsx");
                Console.WriteLine("BaseFieldIndex has been demonstrated successfully.");
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

* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


