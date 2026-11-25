---
title: "ListObject.ShowTableStyleLastColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Indica se l'ultima colonna nella tabella è a cui è applicato lo stile"
type: docs
url: /it/net/aspose.cells.tables/listobject/showtablestylelastcolumn/
---
## ListObject.ShowTableStyleLastColumn property

Indica se l'ultima colonna nella tabella è lo stile applicato a.

```csharp
public bool ShowTableStyleLastColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleLastColumnDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Crea un oggetto elenco
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Imposta la proprietà ShowTableStyleLastColumn
            listObject.ShowTableStyleLastColumn = true;

            // Salva la cartella di lavoro
            workbook.Save("ListObjectShowLastColumnStyle.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("File saved with ShowTableStyleLastColumn enabled.");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


