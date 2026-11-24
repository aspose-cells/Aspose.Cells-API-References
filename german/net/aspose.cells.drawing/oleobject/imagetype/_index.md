---
title: "OleObject.ImageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt das Bildformat des Ole-Objekts zurück"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/imagetype/
---
## OleObject.ImageType property

Liest das Bildformat des OleObject.

```csharp
public ImageType ImageType { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein OLE-Objekt zum Arbeitsblatt hinzufügen
            byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Zeigt den aktuellen Bildtyp des OLE-Objekts an
            Console.WriteLine("Current ImageType value: " + oleObject.ImageType);

            // Demonstriert, wie die ImageType-Eigenschaft verwendet wird
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

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectImageTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


