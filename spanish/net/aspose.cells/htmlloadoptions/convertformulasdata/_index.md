---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. si es true, convierte la cadena a fórmula cuando el valor de cadena comienza con un carácter; el valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

si es true, convierte la cadena a fórmula cuando el valor de cadena comienza con el carácter '=', el valor predeterminado es false.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad HtmlLoadOptions.HasFormula. Esta propiedad será eliminada 12 meses después desde marzo de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // Crea una instancia de HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Establezca la propiedad ConvertFormulasData a true
            options.ConvertFormulasData = true;

            // Cargar un archivo HTML en un Libro de trabajo usando las opciones especificadas
            Workbook workbook = new Workbook("input.html", options);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar algunos valores de celda para demostrar la conversión de fórmulas
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


