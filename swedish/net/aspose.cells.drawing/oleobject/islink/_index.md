---
title: "OleObject.IsLink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Returnerar true om OleObject länkar till filen"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Returnerar true om OleObject länkar till filen.

```csharp
public bool IsLink { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Läs in källarbetsboken
            Workbook workbook = new Workbook("example.xlsm");

            // Bearbeta varje kalkylblad
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // Bearbeta varje OLE-objekt i kalkylbladet
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // Hoppa över om OLE-objektet inte är länkat
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // Visa och ändra den länkade filsökvägen
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // Spara den modifierade arbetsboken
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


