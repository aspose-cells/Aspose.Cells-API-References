---
title: "PasteOptions.OperationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PasteOptions-egenskap. Hämtar och anger operationstypen när ett område klistras in"
type: docs
url: /sv/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Hämtar och anger operationstypen vid inklistring av intervallet.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // Skapa källarbetsbok med exempeldata
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // Skapa målarbetsbok
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // Skapa områden för kopiera/klistra in
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // Skapa klistra in-alternativ med demonstration av OperationType
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // Utför kopiera/klistra in-operationen
            rangeDestination.Copy(rangeOrigin, options);
            
            // Verifiera resultatet
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // Spara resultatet
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


