---
title: "IPageSavingCallback.PageEndSaving"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IPageSavingCallback. Controlar/Indicar que una página termina para ser exportada"
type: docs
url: /es/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

Controla/Indica que una página termina de ser exportada.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | PageEndSavingArgs | La información de una página finaliza el proceso de guardado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y rellenar datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para crear múltiples páginas al renderizarse
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // Crear opciones de guardado PDF con devolución de llamada personalizada de guardado de página
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // Guardar el libro de trabajo con la implementación de la devolución de llamada
                workbook.Save("PageEndSavingDemo.pdf", saveOptions);
                Console.WriteLine("Document saved successfully with page end tracking.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during document save: {ex.Message}");
            }
        }

        private class PageEndSavingCallback : IPageSavingCallback
        {
            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Mostrar información de finalización del guardado de página
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // Puedes agregar operaciones de archivo u otro post-procesamiento aquí
                // args.HasMorePages indica si se procesarán más páginas
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Implementación de interfaz requerida
            }
        }
    }
}
```

### Ver también

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


