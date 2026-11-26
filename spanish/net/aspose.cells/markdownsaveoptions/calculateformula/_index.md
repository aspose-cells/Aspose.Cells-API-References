---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Indica si se deben calcular las fórmulas antes de guardar el archivo markdown"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Indica si se deben calcular las fórmulas antes de guardar el archivo markdown.

```csharp
public bool CalculateFormula { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con fórmulas
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // Crear una instancia de MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Mostrar el valor predeterminado de CalculateFormula
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Establecer CalculateFormula en true para calcular las fórmulas antes de guardar
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Guardar el libro de trabajo con el cálculo de fórmulas habilitado
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Establecer CalculateFormula en false para guardar las fórmulas tal como están
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Guardar el libro de trabajo con el cálculo de fórmulas deshabilitado
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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


