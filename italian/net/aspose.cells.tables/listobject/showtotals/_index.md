---
title: "ListObject.ShowTotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene e imposta se questa tabella mostra la riga dei totali"
type: docs
url: /it/net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Ottiene e imposta se questa TAble mostra la riga totale.

```csharp
public bool ShowTotals { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTotalsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(8);

            // Crea un oggetto elenco/tabella
            int index = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject table = worksheet.ListObjects[index];

            // Abilita la riga dei totali e imposta un calcolo
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Salva la cartella di lavoro
            workbook.Save("ListObjectShowTotalsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


