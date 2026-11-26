---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece el ExportObjectListener para exportar objetos"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Obtiene o establece el ExportObjectListener para exportar objetos.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utiliza la propiedad HtmlSaveOptions.IStreamProvider. Esta propiedad será eliminada 12 meses después desde agosto de 2015. Aspose se disculpa por cualquier inconveniente que puedas haber experimentado.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportObjectListenerDemo
    {
        public static void Run()
        {
            // Crear un listener de exportación de objetos personalizado
            var listener = new CustomExportObjectListener();
            
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // Crear opciones de guardado HTML con el listener
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // Guardar a archivo HTML
            workbook.Save("output.html", saveOptions);
        }
    }

    // Implementación personalizada de IExportObjectListener
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Ejemplo: Procesar el objeto exportado
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // Devolver el objeto original (puede modificarse si es necesario)
            return e;
        }
    }
}
```

### Ver también

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


