---
title: "WarningInfo.CorrectedObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WarningInfo-egenskap. Hämtar och anger det korrigerade objektet"
type: docs
url: /sv/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Hämtar och anger det korrigerade objektet.

```csharp
public object CorrectedObject { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och utlösa en varning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange ett namn som normalt skulle utlösa en varning
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // Hantera varningsåteranrop
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // Denna operation skulle utlösa varningsåteranropet
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // Demonstrera användning av CorrectedObject
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### Se även

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


