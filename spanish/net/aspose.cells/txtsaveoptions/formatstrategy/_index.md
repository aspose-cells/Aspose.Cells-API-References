---
title: "TxtSaveOptions.FormatStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/formatstrategy/
---
## TxtSaveOptions.FormatStrategy property

Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca valores con diferentes formatos
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);

            // Aplique formato numérico a los precios
            Style style = workbook.CreateStyle();
            style.Number = 2; // Format as currency
            worksheet.Cells["B2:B3"].SetStyle(style);

            // Configure las opciones de guardado de texto con diferentes estrategias de formato
            TxtSaveOptions options = new TxtSaveOptions
            {
                Separator = '\t',
                FormatStrategy = CellValueFormatStrategy.DisplayStyle // Show formatted values
            };

            // Guarde con formato de visualización
            workbook.Save("FormattedOutput.txt", options);

            // Cambie a ninguna estrategia de formato
            options.FormatStrategy = CellValueFormatStrategy.None;
            workbook.Save("RawOutput.txt", options);

            Console.WriteLine("Files saved with different format strategies.");
        }
    }
}
```

### Ver también

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


