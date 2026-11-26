---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Indica si las filas en blanco en la hoja de cálculo deben tratarse como separadores de tabla al exportar a Markdown. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

Indica si las filas en blanco en la hoja de cálculo deben tratarse como separadores de tabla al exportar a Markdown. El valor predeterminado es falso.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con filas en blanco para demostrar la división de tablas
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // Agregar una fila en blanco (fila 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // Crear una instancia de MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Mostrar el valor predeterminado de SplitTablesByBlankRow
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Establecer SplitTablesByBlankRow a true para dividir las tablas por filas en blanco
                saveOptions.SplitTablesByBlankRow = true;

                // Mostrar el valor actualizado
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Guardar el libro de trabajo como markdown con la división de tablas habilitada
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


