---
title: "ConditionalFormattingIcon.ImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingIcon. Obtiene los datos del conjunto de íconos"
type: docs
url: /es/net/aspose.cells/conditionalformattingicon/imagedata/
---
## ConditionalFormattingIcon.ImageData property

Obtiene los datos del conjunto de íconos.

```csharp
public byte[] ImageData { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo y formato condicional
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Obtener el resultado del formato condicional
            var conditionalFormattingResult = worksheet.Cells["A1"].GetConditionalFormattingResult();
            if (conditionalFormattingResult != null)
            {
                ConditionalFormattingIcon icon = conditionalFormattingResult.ConditionalFormattingIcon;
                if (icon != null)
                {
                    // Obtener los datos de la imagen del ícono
                    byte[] imageData = icon.ImageData;
                    
                    // Verificar y mostrar la información de la imagen
                    if (imageData != null && imageData.Length > 0)
                    {
                        Console.WriteLine($"Icon data length: {imageData.Length} bytes");
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


