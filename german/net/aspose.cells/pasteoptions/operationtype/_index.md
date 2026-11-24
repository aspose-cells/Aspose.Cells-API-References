---
title: "PasteOptions.OperationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PasteOptions-Eigenschaft. Liest und setzt den Operationstyp beim Einfügen eines Bereichs"
type: docs
url: /de/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Liest und setzt den Operationstyp beim Einfügen des Bereichs.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Quell-Arbeitsmappe mit Beispieldaten.
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // Erstelle Ziel‑Arbeitsbuch
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // Erstelle Bereiche für Kopieren/Einfügen
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // Erstelle PasteOptions mit Demonstration von OperationType
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // Führe die Kopieren/Einfügen-Operation aus
            rangeDestination.Copy(rangeOrigin, options);
            
            // Überprüfe das Ergebnis
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // Ergebnis speichern
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


