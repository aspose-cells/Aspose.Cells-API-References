---
title: "ListObject.StartRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene la riga iniziale dell'intervallo"
type: docs
url: /it/net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Ottiene la riga iniziale dell'intervallo.

```csharp
public int StartRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio a partire dalla riga 2
            worksheet.Cells["A2"].PutValue("ID");
            worksheet.Cells["B2"].PutValue("Name");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue("John");
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["B4"].PutValue("Mary");

            // Crea un oggetto elenco a partire dalla riga 2
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Visualizza la proprietà StartRow
            Console.WriteLine("ListObject StartRow: " + listObject.StartRow);

            // Per "modificare" la riga iniziale, dobbiamo ricreare il ListObject
            worksheet.ListObjects.RemoveAt(listObjectIndex);
            listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
            listObject = worksheet.ListObjects[listObjectIndex];
            
            Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


