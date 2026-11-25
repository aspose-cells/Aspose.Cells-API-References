---
title: "PivotTable.SourceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene il tipo di origine dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/sourcetype/
---
## PivotTable.SourceType property

Ottiene il tipo di origine dati della tabella pivot.

```csharp
public PivotTableSourceType SourceType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertySourceTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Product A";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Product B";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Product C";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di SourceType
            Console.WriteLine("Current PivotTable SourceType: " + pivotTable.SourceType);

            // Calcola i dati per mostrare la tabella pivot
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableSourceTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotTableSourceType](../../pivottablesourcetype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


