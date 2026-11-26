---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Indica si se debe comprobar la compatibilidad de fuentes para cada carácter en el texto.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Observaciones

El valor predeterminado es true. Desactivar esta propiedad puede ofrecer mejor rendimiento. Pero cuando la fuente predeterminada o especificada del texto/caracter no puede usarse para renderizarlo, pueden aparecer caracteres ilegibles (como bloques) en el PDF generado. En tal situación, el usuario debe mantener esta propiedad en true para que se busque y utilice una fuente alternativa para renderizar el texto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // Cree opciones de guardado paginadas
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Demuestre la propiedad CheckFontCompatibility
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // Establezca otras propiedades requeridas
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // Guarde el documento con las opciones especificadas
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


