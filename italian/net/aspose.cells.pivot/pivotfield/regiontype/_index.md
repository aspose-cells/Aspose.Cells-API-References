---
title: "PivotField.RegionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotField proprietà. Specifica la regione della tabella pivot in cui questo campo è visualizzato"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

Specifica la regione della tabella pivot in cui viene visualizzato questo campo.

```csharp
public PivotFieldType RegionType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crea una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ottieni il primo campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // Visualizza il valore corrente di RegionType
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // Dimostra come utilizzare la proprietà RegionType
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


