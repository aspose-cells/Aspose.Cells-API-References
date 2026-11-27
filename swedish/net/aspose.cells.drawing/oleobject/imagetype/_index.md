---
title: "OleObject.ImageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject egenskap. Hämtar bildformatet för ole-objektet"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/imagetype/
---
## OleObject.ImageType property

Hämtar bildformatet för ole-objektet.

```csharp
public ImageType ImageType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OLE‑objekt i kalkylbladet
            byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Visa den aktuella bildtypen för OLE-objektet
            Console.WriteLine("Current ImageType value: " + oleObject.ImageType);

            // Demonstrera hur man använder ImageType-egenskapen
            if (oleObject.ImageType == ImageType.Unknown)
            {
                Console.WriteLine("The OLE object's image format is not recognized.");
            }
            else if (oleObject.ImageType == ImageType.Emf)
            {
                Console.WriteLine("The OLE object uses EMF image format.");
            }
            else if (oleObject.ImageType == ImageType.Png)
            {
                Console.WriteLine("The OLE object uses PNG image format.");
            }

            // Spara arbetsboken
            workbook.Save("OleObjectImageTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


