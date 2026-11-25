---
title: "PivotShowValuesSetting.CalculationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotShowValuesSetting. Rappresenta come visualizzare i valori di un campo dati nel report pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotshowvaluessetting/calculationtype/
---
## PivotShowValuesSetting.CalculationType property

Rappresenta come visualizzare i valori di un campo dati nel report pivot.

```csharp
[Obsolete("Use PivotShowValuesSetting.ShowValuesAs property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotShowValuesSetting.ShowValuesAs. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyCalculationTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Aggiungi il campo dati e imposta il tipo di calcolo
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.RankLargestToSmallest;

            // Calcola i dati e salva
            pivotTable.CalculateData();
            workbook.Save("PivotShowValuesSettingPropertyCalculationTypeDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


