---
title: "ListColumnCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumnCollection‑egenskap. Hämtar ListColumn efter index"
type: docs
url: /sv/net/aspose.cells.tables/listcolumncollection/item/
---
## ListColumnCollection indexer (1 of 2)

Hämtar ListColumn efter index.

```csharp
public ListColumn this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

ListColumn‑objektet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("T1");
            worksheet.Cells["B1"].PutValue("T2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            
            // Åtkomst till listkolumner med Item‑egenskapen
            ListColumn firstColumn = listObj.ListColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListColumnCollection indexer (2 of 2)

Hämtar ListColumn efter namn.

```csharp
public ListColumn this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på ListColumn |

### Returvärde

ListColumn‑objektet.

### Se även

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


