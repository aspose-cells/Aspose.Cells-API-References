---
title: "PivotArea.AxisType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotArea. Ottiene e imposta la regione della PivotTable a cui si applica questa regola"
type: docs
url: /it/net/aspose.cells.pivot/pivotarea/axistype/
---
## PivotArea.AxisType property

Ottiene e imposta la regione della PivotTable a cui si applica questa regola.

```csharp
public PivotFieldType AxisType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyAxisTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 800;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alle aree pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Sales

            // Crea e configura PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row; // Demonstrate AxisType property
            pivotArea.RuleType = PivotAreaType.Normal;

            // Seleziona l'area pivot
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Salva la cartella di lavoro
            workbook.Save("PivotAreaAxisTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


