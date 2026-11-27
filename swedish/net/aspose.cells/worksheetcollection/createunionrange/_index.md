---
title: "WorksheetCollection.CreateUnionRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Skapar ett Range-objekt från en adress för intervallet."
type: docs
url: /sv/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Skapar ett [`Range`](../../range/) objekt från en adress för intervallet.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adress | String | Adressen för intervallet. |
| sheetIndex | Int32 | Bladindexet. |

### Returvärde

Ett [`Range`](../../range/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett förenat område från adresssträngar
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Ange värde för hela unionområdet
            unionRange.Value = "Test";
            
            // Tillämpa stil på unionområdet
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // Spara arbetsboken
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


