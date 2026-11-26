---
title: "HtmlSaveOptions.CssStyles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece los estilos css adicionales para el formateador. Solo funciona cuando SaveAsSingleFile es True.  CssStylesbody  padding 5px"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

Obtiene o establece los estilos css adicionales para el formateador. Solo funciona cuando [`SaveAsSingleFile`](../saveassinglefile/) es True.  CssStyles="body { padding: 5px }";

```csharp
public string CssStyles { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCssStylesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer estilos CSS personalizados
            saveOptions.CssStyles = @"
                body { 
                    font-family: Arial;
                    background-color: #f0f0f0;
                }
                table {
                    border-collapse: collapse;
                    width: 100%;
                }
                td {
                    border: 1px solid #ddd;
                    padding: 8px;
                }";

            // Guardar el libro de trabajo con estilos CSS personalizados
            workbook.Save("HtmlWithCustomStyles.html", saveOptions);

            Console.WriteLine("HTML file with custom CSS styles created successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


