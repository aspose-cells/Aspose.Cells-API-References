---
title: "OleObject.ImageSourceFullName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Obtiene o establece la ruta y el nombre del archivo fuente para la imagen vinculada"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Obtiene o establece la ruta y el nombre del archivo fuente para la imagen vinculada.

```csharp
public string ImageSourceFullName { get; set; }
```

### Observaciones

El valor predeterminado es una cadena vacía. Si SourceFullName no es una cadena vacía, la imagen está vinculada. Si SourceFullName no es una cadena vacía, pero Data es nulo, entonces la imagen está vinculada y no se almacena en el archivo.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Archivo PDF de ejemplo para incrustar
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // Agregar un OleObject a la hoja de cálculo
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // Establezca propiedades OleObject incluyendo ImageSourceFullName
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // Guarda el libro de trabajo
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


