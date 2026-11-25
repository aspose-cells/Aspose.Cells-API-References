---
title: "ListObject.Comment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene e imposta il commento della tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

Ottiene e imposta il commento della tabella.

```csharp
public string Comment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per l'oggetto lista
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(100);

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];

            // Imposta e dimostra la proprietà Comment
            listObj.Comment = "This is a sample comment for the list object";
            Console.WriteLine("List Object Comment: " + listObj.Comment);

            // Ridimensiona l'oggetto lista per includere più dati
            listObj.Resize(0, 0, 2, 1, true);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(200);

            // Salva la cartella di lavoro
            workbook.Save("ListObjectCommentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


