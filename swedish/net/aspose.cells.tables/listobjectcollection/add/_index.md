---
title: "ListObjectCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObjectCollection-metod. Lägger till ett ListObject i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Lägger till ett ListObject i kalkylbladet.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden för listområdet. |
| startColumn | Int32 | Startraden för listområdet. |
| endRow | Int32 | Startraden för listområdet. |
| endColumn | Int32 | Startraden för listområdet. |
| hasHeaders | Boolean | Om området har rubriker. |

### Returvärde

Index för den nya ListObject

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i data i ett område
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // Lägg till ListObject med Add-metoden och Int32-parametrar
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Aktivera totaler och ange formel för en kolumn
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // Spara arbetsboken
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Lägger till ett ListObject i kalkylbladet.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startCell | String | Startcellen i listområdet. |
| endCell | String | Slutcellen i listområdet. |
| hasHeaders | Boolean | Om området har rubriker. |

### Returvärde

Index för den nya ListObject

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i exempeldata
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // Lägg till listobjekt med strängområdesreferenser
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Se även

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


