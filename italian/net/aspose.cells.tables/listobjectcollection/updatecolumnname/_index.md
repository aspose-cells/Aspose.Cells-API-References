---
title: "ListObjectCollection.UpdateColumnName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObjectCollection. Aggiorna tutti i nomi delle colonne delle tabelle"
type: docs
url: /it/net/aspose.cells.tables/listobjectcollection/updatecolumnname/
---
## ListObjectCollection.UpdateColumnName method

Aggiorna tutti i nomi delle colonne delle tabelle.

```csharp
public void UpdateColumnName()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ListObjectCollection listObjects = worksheet.ListObjects;
            int listObjectIndex = listObjects.Add(0, 0, 10, 4, true);
            ListObject listObject = listObjects[listObjectIndex];
            listObject.DisplayName = "SampleTable";

            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["D1"].PutValue("Total");

            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Product " + i);
                worksheet.Cells[i, 1].PutValue(i * 10);
                worksheet.Cells[i, 2].PutValue(i);
                worksheet.Cells[i, 3].PutValue(i * i * 10);
            }

            listObjects.UpdateColumnName();

            workbook.Save("ListObjectUpdateColumnNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


