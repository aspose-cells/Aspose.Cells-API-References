---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece la resolución predeterminada de la imagen"
type: docs
url: /es/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

Obtiene y establece la resolución predeterminada de la imagen.

```csharp
public int DefaultImageResolution { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer la resolución predeterminada de la imagen
            workbook.Settings.DefaultImageResolution = 300;
            
            // Agregar una hoja de cálculo e insertar una imagen
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verificar la resolución predeterminada de la imagen
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


