---
title: "PivotAreaFilter.Selected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotAreaFilter. Indica se questo campo ha una selezione. Funziona solo quando la PivotTable è in visualizzazione Outline"
type: docs
url: /it/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

Indica se questo campo ha una selezione. Funziona solo quando la PivotTable è in visualizzazione Schema.

```csharp
public bool Selected { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crea una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ottieni il filtro dell'area pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // Visualizza il valore Selected corrente
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // Modifica il valore Selected (influisce solo sulla visualizzazione Outline)
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // Salva la cartella di lavoro
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


