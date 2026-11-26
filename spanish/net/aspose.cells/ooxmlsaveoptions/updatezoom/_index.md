---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OoxmlSaveOptions. Indica si se actualiza el factor de escala antes de guardar el archivo cuando las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

Indica si se actualiza el factor de escala antes de guardar el archivo cuando las propiedades PageSetup.FitToPagesWide y PageSetup.FitToPagesTall controlan cómo se escala la hoja de cálculo.

```csharp
public bool UpdateZoom { get; set; }
```

### Observaciones

El valor predeterminado es false por rendimiento.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyUpdateZoomDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer nivel de zoom inicial
            worksheet.PageSetup.Zoom = 100;

            // Crear opciones de guardado con UpdateZoom habilitado
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // Guardar en flujo de memoria
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Recargar el libro de trabajo para verificar que el zoom se haya actualizado
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### Ver también

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


