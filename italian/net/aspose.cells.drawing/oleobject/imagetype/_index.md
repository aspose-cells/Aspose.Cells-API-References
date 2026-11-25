---
title: "OleObject.ImageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Ottiene il formato immagine dell'oggetto ole"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/imagetype/
---
## OleObject.ImageType property

Ottiene il formato immagine dell'oggetto ole.

```csharp
public ImageType ImageType { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un oggetto OLE al foglio di lavoro
            byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Visualizza il tipo di immagine corrente dell'oggetto OLE
            Console.WriteLine("Current ImageType value: " + oleObject.ImageType);

            // Dimostra come utilizzare la proprietà ImageType
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

            // Salva la cartella di lavoro
            workbook.Save("OleObjectImageTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


