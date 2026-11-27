---
title: "OleObject.Label"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject egenskap. Hämtar och anger visningsetiketten för det länkade ole-objektet"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Hämtar och anger visningsetiketten för det länkade ole-objektet.

```csharp
public string Label { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyLabelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OLE-objekt med en etikett
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // Spara och ladda om arbetsboken
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // Verifiera label-egenskapen
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


