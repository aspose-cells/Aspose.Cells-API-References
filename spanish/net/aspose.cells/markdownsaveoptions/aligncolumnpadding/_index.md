---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Indica si la alineación de columnas está habilitada para las tablas Markdown generadas. Cuando está habilitada, las columnas se alinean rellenando el contenido de la celda con el carácter especificado, típicamente espacios. Establezca 0 para desactivar la alineación de columnas por defecto"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Indica si la alineación de columnas está habilitada para las tablas Markdown generadas. Cuando está habilitada, las columnas se alinean rellenando el contenido de la celda con el carácter especificado (normalmente ' ' para espacios). Establezca '\0' para desactivar la alineación de columnas (valor predeterminado).

```csharp
public char AlignColumnPadding { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para demostrar la alineación de columnas
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // Crear una instancia de MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Mostrar el valor predeterminado de AlignColumnPadding
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Establecer AlignColumnPadding al carácter de espacio para la alineación de columnas
                saveOptions.AlignColumnPadding = ' ';

                // Mostrar el valor actualizado
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Guardar el libro de trabajo como markdown con alineación de columnas
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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


