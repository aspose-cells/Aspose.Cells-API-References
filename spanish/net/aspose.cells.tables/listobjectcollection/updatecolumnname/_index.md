---
title: "ListObjectCollection.UpdateColumnName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListObjectCollection. Actualizar todos los nombres de columna de las tablas"
type: docs
url: /es/net/aspose.cells.tables/listobjectcollection/updatecolumnname/
---
## ListObjectCollection.UpdateColumnName method

Actualizar todos los nombres de columna de las tablas.

```csharp
public void UpdateColumnName()
```

### Ejemplos

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

### Ver también

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


