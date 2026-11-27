---
title: "WorksheetCollection.Insert"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Infoga ett arbetsblad"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Infoga ett kalkylblad.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Bladets index |
| sheetType | SheetType | Bladtypen. |

### Returvärde

Returnerar ett infogat arbetsblad.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Infoga ett kalkylblad.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Bladets index |
| sheetType | SheetType | Bladtypen. |
| sheetName | String | Bladnamnet. |

### Returvärde

Returnerar ett infogat arbetsblad.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Infoga ett nytt arbetsblad på index 0 med namnet "InsertedSheet"
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // Kom åt det infogade arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sätt in lite data i cell A1 på det infogade bladet
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // Spara arbetsboken
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


