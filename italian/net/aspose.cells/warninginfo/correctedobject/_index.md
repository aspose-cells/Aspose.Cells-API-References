---
title: "WarningInfo.CorrectedObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WarningInfo. Ottiene e imposta l'oggetto corretto"
type: docs
url: /it/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Ottiene e imposta l'oggetto corretto.

```csharp
public object CorrectedObject { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e genera un avviso
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta un nome che normalmente genererebbe un avviso
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // Gestisci la callback di avviso
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // Questa operazione attiverebbe la callback di avviso
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // Dimostra l'uso di CorrectedObject
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### Vedi anche

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


