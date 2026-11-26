---
title: "OdsPageBackground.GraphicData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsPageBackground. Obtiene y establece los datos del gráfico"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/graphicdata/
---
## OdsPageBackground.GraphicData property

Obtiene y establece los datos gráficos.

```csharp
public byte[] GraphicData { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y su configuración de página
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer propiedades de fondo de página ODS
            OdsPageBackground background = pageSetup.ODSPageBackground;
            background.Type = OdsPageBackgroundType.Graphic;
            
            // Cargar datos de imagen y establecer como fondo
            string imagePath = "sample.png"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                background.GraphicData = File.ReadAllBytes(imagePath);
                background.GraphicType = OdsPageBackgroundGraphicType.Area;
                
                // Guarda el libro de trabajo
                workbook.Save("output.ods");
                
                Console.WriteLine("ODS file with graphic background created successfully.");
            }
            else
            {
                Console.WriteLine("Image file not found: " + imagePath);
            }
        }
    }
}
```

### Ver también

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


