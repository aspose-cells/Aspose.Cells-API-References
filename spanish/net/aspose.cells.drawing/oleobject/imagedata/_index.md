---
title: "OleObject.ImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Representa la imagen del objeto ole como una matriz de bytes"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Representa la imagen del objeto ole como una matriz de bytes.

```csharp
public byte[] ImageData { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Leer el archivo de imagen en una matriz de bytes
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // Agregar objeto OLE con los datos de la imagen
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // Establecer propiedades del objeto incrustado
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // Demostrar el uso de la propiedad ImageData
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // Guarda el libro de trabajo
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


