---
title: "ListObject.AlternativeText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene e imposta il testo alternativo"
type: docs
url: /it/net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

Ottiene e imposta il testo alternativo.

```csharp
public string AlternativeText { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un oggetto elenco/tabella
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Imposta testo alternativo e descrizione
            table.AlternativeText = "Test";
            table.AlternativeDescription = "aSXADCS";
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Ricarica e verifica
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


