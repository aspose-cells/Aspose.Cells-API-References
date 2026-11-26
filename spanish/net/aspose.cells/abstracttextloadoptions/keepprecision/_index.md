---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractTextLoadOptions. Indica si no se analiza un valor de cadena cuando la longitud es 15"
type: docs
url: /es/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Indica si no se analiza un valor de cadena cuando la longitud es 15.

```csharp
public bool KeepPrecision { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML y establecer KeepPrecision en true
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // Cargue el libro de trabajo con las opciones
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Demostrar que la precisión se mantiene (p.ej., valores numéricos con muchos decimales)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


