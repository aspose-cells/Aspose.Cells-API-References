---
title: "ListObject.ApplyStyleToRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Applica lo stile della tabella all'intervallo"
type: docs
url: /it/net/aspose.cells.tables/listobject/applystyletorange/
---
## ListObject.ApplyStyleToRange method

Applica lo stile di tabella all'intervallo.

```csharp
public void ApplyStyleToRange()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodApplyStyleToRangeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare un oggetto elenco
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = worksheet.ListObjects[index];

            // Applica lo stile all'intervallo dell'oggetto elenco
            listObject.ApplyStyleToRange();

            // Verifica che lo stile sia stato applicato controllando il colore di primo piano di una cella
            Style style = worksheet.Cells["A1"].GetStyle();
            Console.WriteLine("Foreground color applied: " + style.ForegroundColor);

            // Converti l'oggetto elenco in intervallo e verifica
            listObject.ConvertToRange();
            Console.WriteLine("List objects count after conversion: " + worksheet.ListObjects.Count);
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


