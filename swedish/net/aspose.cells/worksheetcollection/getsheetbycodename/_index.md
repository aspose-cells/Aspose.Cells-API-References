---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Hämtar bladet efter kodnamnet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Hämtar kalkylbladet efter kodnamnet.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| codeName | String | Kodnamn för bladet. |

### Returvärde

Elementet med det angivna kodnamnet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till kalkylblad och ange deras kodnamn
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // Hämta kalkylblad efter kodnamn
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // Demonstrera användning genom att skriva till celler
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // Spara arbetsboken
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


