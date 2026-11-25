---
title: "ListObject.AlternativeDescription"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene e imposta la descrizione alternativa"
type: docs
url: /it/net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Ottiene e imposta la descrizione alternativa.

```csharp
public string AlternativeDescription { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeDescriptionDemo
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

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Imposta testo alternativo e descrizione
            listObject.AlternativeText = "Test";
            listObject.AlternativeDescription = "aSXADCS";

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Ricarica e verifica le proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


