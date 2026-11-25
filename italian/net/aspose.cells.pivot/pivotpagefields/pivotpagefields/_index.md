---
title: "PivotPageFields.PivotPageFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore PivotPageFields. Rappresenta gli elementi del campo pagina pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Rappresenta gli elementi del campo di pagina della pivot.

```csharp
public PivotPageFields()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // Crea campi pagina pivot utilizzando il costruttore
            PivotPageFields pageFields = new PivotPageFields();
            
            // Aggiungi campi pagina
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // Aggiungi identificazione
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // Aggiungi tabella pivot con i parametri corretti
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // Salva la cartella di lavoro
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


