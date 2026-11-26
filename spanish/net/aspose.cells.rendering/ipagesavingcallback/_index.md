---
title: "Interfaz IPageSavingCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Rendering.IPageSavingCallback interface. Controla/Indica el progreso del proceso de guardado de página"
type: docs
url: /es/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

Controlar/Indicar el progreso del proceso de guardado de la página.

```csharp
public interface IPageSavingCallback
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Controla/Indica que una página termina de ser exportada. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Controla/Indica que una página comienza a ser exportada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingCallbackDemo : IPageSavingCallback
    {
        public static void PageSavingCallbackExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Cree opciones de guardado con una devolución de llamada de guardado de página
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Guarde el libro de trabajo como archivo DOCX
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // Implemente el método PageStartSaving
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // Implemente el método PageEndSaving
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


