---
title: "PaginatedSaveOptions.DefaultEditLanguage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece el idioma de edición predeterminado"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

Obtiene o establece el idioma de edición predeterminado.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Observaciones

Puede mostrar/renderizar diferentes diseños para párrafos de texto cuando se establece un idioma de edición diferente. El predeterminado es Auto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue algo de texto CJK para demostrar la propiedad DefaultEditLanguage
            worksheet.Cells["A1"].PutValue("日本語のテキスト");
            worksheet.Cells["A2"].PutValue("中文文本");
            worksheet.Cells["A3"].PutValue("한글 텍스트");

            // Cree opciones de guardado PDF y establezca CJK como idioma de edición predeterminado
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            
            // Guardar el libro de trabajo con las opciones especificadas
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("Workbook saved with CJK as default edit language.");
        }
    }
}
```

### Ver también

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


