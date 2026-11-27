---
title: "ListObjectCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObjectCollection-egenskap. Hämtar ListObject efter index"
type: docs
url: /sv/net/aspose.cells.tables/listobjectcollection/item/
---
## ListObjectCollection indexer (1 of 2)

Hämtar ListObject efter index.

```csharp
public ListObject this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Den ListObject

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Åtkomst till listobjekt med Item-egenskapen
            ListObject firstListObject = worksheet.ListObjects[0];
            
            // Ange tabellstil
            firstListObject.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListObjectCollection indexer (2 of 2)

Hämtar ListObject efter angivet namn.

```csharp
public ListObject this[string tableName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| tableName | ListObject namn. |

### Returvärde

Den ListObject

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.DisplayName = "PersonTable";

            // Åtkomst till listobjektet med Item-egenskapen efter namn
            ListObject retrievedListObj = worksheet.ListObjects["PersonTable"];
            
            // Demonstrera användning genom att konvertera till område
            retrievedListObj.ConvertToRange();

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


