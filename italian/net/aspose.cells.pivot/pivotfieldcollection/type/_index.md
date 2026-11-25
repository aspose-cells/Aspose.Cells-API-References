---
title: "PivotFieldCollection.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldCollection. Ottiene il tipo di PivotFields"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldcollection/type/
---
## PivotFieldCollection.Type property

Ottiene il tipo di PivotFields.

```csharp
public PivotFieldType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Visualizza il tipo della pivot field collection
            Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotFieldCollection dataFields = pivotTable.DataFields;

            // Visualizza il tipo della data field collection
            Console.WriteLine("DataFields Type: " + dataFields.Type);

            // Calcola i dati e aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva il risultato
            workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


