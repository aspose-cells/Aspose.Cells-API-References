---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownLoadOptions. Indica si el texto es una fórmula si comienza con"
type: docs
url: /es/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Indica si el texto es una fórmula si comienza con "=".

```csharp
public bool HasFormula { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una instancia de MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Mostrar el valor predeterminado de HasFormula
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // Establecer HasFormula a verdadero
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Establecer HasFormula a falso
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Crear un libro de trabajo con contenido markdown de ejemplo
                Workbook workbook = new Workbook();

                // Guardar el libro de trabajo para demostrar que se pueden usar las opciones
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
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

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


