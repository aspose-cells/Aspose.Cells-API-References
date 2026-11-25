---
title: "Classe PivotAreaFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotAreaFilter. Rappresenta il filtro di PivotArea per PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

Rappresenta il filtro di [`PivotArea`](../pivotarea/) per [`PivotTable`](../pivottable/).

```csharp
public class PivotAreaFilter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | Ottiene l'indice del campo nei campi di origine a cui si riferisce questo filtro. Un valore di -2 indica il campo dei valori. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Indica se questo campo ha una selezione. Funziona solo quando la PivotTable è in visualizzazione Schema. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Ottiene quale subtotale è impostato per questo filtro. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Subtotale per il filtro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configurazione dati di esempio
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // Crea PivotTable - correggi la gestione del valore di ritorno
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Crea e configura PivotAreaFilter
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // Dimostra i metodi
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


