---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad WorkbookSettings. Indica si se descartan los datos de edición de imágenes"
type: docs
url: /es/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Indica si se descarta la edición de datos de imagen.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una imagen a la hoja de cálculo
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Establece DiscardImageEditData a true (el valor predeterminado es false)
            workbook.Settings.DiscardImageEditData = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // Verifique que la configuración se haya aplicado
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


