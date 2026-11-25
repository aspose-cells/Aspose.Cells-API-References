---
title: "PivotTable.AltTextDescription"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene la descrizione del testo alternativo"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/alttextdescription/
---
## PivotTable.AltTextDescription property

Ottiene la descrizione del testo alternativo.

```csharp
public string AltTextDescription { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextDescriptionDemo
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
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza la descrizione attuale del testo alternativo
            Console.WriteLine("Current AltTextDescription: " + pivotTable.AltTextDescription);

            // Imposta una nuova descrizione del testo alternativo
            pivotTable.AltTextDescription = "Sales data by product category";

            // Salva la cartella di lavoro
            workbook.Save("PivotTableAltTextDescriptionDemo.xlsx");

            // Visualizza la nuova descrizione del testo alternativo
            Console.WriteLine("New AltTextDescription: " + pivotTable.AltTextDescription);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


