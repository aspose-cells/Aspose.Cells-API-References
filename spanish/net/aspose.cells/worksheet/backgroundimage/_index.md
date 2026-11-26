---
title: "Worksheet.BackgroundImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene y establece la imagen de fondo de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Obtiene y establece la imagen de fondo de la hoja de cálculo.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyBackgroundImageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ruta al archivo de imagen
            string imagePath = "background.jpg";
            
            // Leer el archivo de imagen en una matriz de bytes
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Establecer la imagen de fondo para la hoja de cálculo
            worksheet.BackgroundImage = imageData;
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


