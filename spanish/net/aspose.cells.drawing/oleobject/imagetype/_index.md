---
title: "OleObject.ImageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Obtiene el formato de imagen del objeto ole"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/imagetype/
---
## OleObject.ImageType property

Obtiene el formato de imagen del objeto ole.

```csharp
public ImageType ImageType { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un objeto OLE a la hoja de cálculo
            byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Muestre el tipo de imagen actual del objeto OLE
            Console.WriteLine("Current ImageType value: " + oleObject.ImageType);

            // Demuestre cómo usar la propiedad ImageType
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

            // Guarda el libro de trabajo
            workbook.Save("OleObjectImageTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


