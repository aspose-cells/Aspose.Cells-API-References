---
title: "ListObject.PutCellValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject metod. Placera värdet i cellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

Placera värdet i cellen.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | Radoffseten i tabellen. |
| columnOffset | Int32 | Kolumnoffseten i tabellen. |
| värde | Object | Cellvärdet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Demonstrera PutCellValue med Int32, Int32, Object-parametrar
            listObject.PutCellValue(1, 0, 500); // Update row 1, column 0 with value 500
            listObject.PutCellValue(1, 1, "Updated Value"); // Update row 1, column 1 with string
            listObject.PutCellValue(1, 2, DateTime.Now); // Update row 1, column 2 with current date

            // Spara arbetsboken
            workbook.Save("ListObjectPutCellValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

Placera värdet i cellen.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | Radoffseten i tabellen. |
| columnOffset | Int32 | Kolumnoffseten i tabellen. |
| värde | Object | Cellvärdet. |
| isTotalsRowLabel | Boolean | Indikerar om det är en etikett för totalraden, fungerar endast för totalraden. Om False och denna rad är totalrad, kommer en ny rad att infogas. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa ett ListObject
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Skapa ett ListObject
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Använd PutCellValue för att uppdatera en cell (rad 2, kolumn 1) med ett nytt värde och expandera tabellen
            listObject.PutCellValue(2, 1, "Updated Value", true);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


