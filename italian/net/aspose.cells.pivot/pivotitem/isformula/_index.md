---
title: "PivotItem.IsFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Indica se questo elemento pivot è un elemento di formula calcolata"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

Indica se questo elemento pivot è un elemento di formula calcolata.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotItem.IsCalculatedItem. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
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
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ottieni il primo elemento pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Visualizza il valore corrente di IsFormula (proprietà obsoleta)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // Imposta un nuovo valore per IsFormula (proprietà obsoleta)
            pivotItem.IsFormula = true;

            // Dimostra l'effetto - questo contrassegnerebbe l'elemento pivot come elemento di formula
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // Nota: Nell'uso reale, dovresti usare IsCalculatedItem invece poiché IsFormula è obsoleta
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // Salva il risultato
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


