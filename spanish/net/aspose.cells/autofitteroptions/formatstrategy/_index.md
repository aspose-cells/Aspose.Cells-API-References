---
title: "AutoFitterOptions.FormatStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Obtiene y establece la estrategia de formato"
type: docs
url: /es/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Obtiene y establece la estrategia de formato.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Observaciones

El valor predeterminado es CellStyle por rendimiento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra y ajustar texto
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Crear AutoFitterOptions con FormatStrategy
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // Aplicar ajuste automático con las opciones especificadas
            worksheet.AutoFitRows(options);

            // Guardar el resultado
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


