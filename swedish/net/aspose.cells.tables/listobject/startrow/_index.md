---
title: "ListObject.StartRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject‑egenskap. Hämtar startraden i intervallet"
type: docs
url: /sv/net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Hämtar startraden i intervallet.

```csharp
public int StartRow { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata med början på rad 2
            worksheet.Cells["A2"].PutValue("ID");
            worksheet.Cells["B2"].PutValue("Name");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue("John");
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["B4"].PutValue("Mary");

            // Skapa ett listobjekt med början på rad 2
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Visa StartRow-egenskapen
            Console.WriteLine("ListObject StartRow: " + listObject.StartRow);

            // För att "modifiera" startraden måste vi återskapa ListObject
            worksheet.ListObjects.RemoveAt(listObjectIndex);
            listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
            listObject = worksheet.ListObjects[listObjectIndex];
            
            Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


