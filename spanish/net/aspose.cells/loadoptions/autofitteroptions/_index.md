---
title: "LoadOptions.AutoFitterOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene y establece las opciones de ajuste automático"
type: docs
url: /es/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Obtiene y establece las opciones del ajuste automático

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Observaciones

Solo para archivos xlsx, SpreadsheetML por ahora.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crear AutoFitterOptions y establecer propiedades
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // Crear LoadOptions y asignar AutoFitterOptions
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // Cargar el libro de trabajo con las opciones especificadas
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // Demostrar el ajuste automático obteniendo la altura de la fila
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


