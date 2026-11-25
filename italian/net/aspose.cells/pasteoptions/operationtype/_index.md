---
title: "PasteOptions.OperationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PasteOptions. Ottiene e imposta il tipo di operazione durante l'incollaggio dell'intervallo"
type: docs
url: /it/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Ottiene e imposta il tipo di operazione durante l'incollaggio dell'intervallo.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di origine con dati di esempio
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // Crea la cartella di lavoro di destinazione
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // Crea intervalli per copia/incolla
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // Crea opzioni di incolla con dimostrazione di OperationType
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // Esegui l'operazione di copia/incolla
            rangeDestination.Copy(rangeOrigin, options);
            
            // Verifica il risultato
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // Salva il risultato
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


