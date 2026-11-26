---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Especifica un valor booleano que indica que la aplicación comprime automáticamente las imágenes en el libro"
type: docs
url: /es/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Especifica un valor booleano que indica que la aplicación comprime automáticamente las imágenes en el libro de trabajo.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Habilitar AutoCompressPictures
            workbook.Settings.AutoCompressPictures = true;
            
            // Agregar una imagen de ejemplo para demostrar la compresión
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargar el libro guardado para verificar la configuración
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


