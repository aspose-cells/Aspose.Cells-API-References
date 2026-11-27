---
title: "PivotItem.GetStringValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-metod. Hämtar strängvärdet för pivot-elementet. Om värdet är null returneras"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Hämtar strängvärdet för pivotobjektet. Om värdet är null, returneras ""

```csharp
public string GetStringValue()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Få åtkomst till det första kalkylbladet och pivottabellen
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Hämta det första radfältet och dess pivot-element
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // Demonstrera GetStringValue()-metoden
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // Spara den modifierade arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


