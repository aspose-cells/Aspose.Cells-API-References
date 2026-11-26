---
title: "LoadOptions.WarningCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene o establece la devolución de llamada de advertencia"
type: docs
url: /es/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Obtiene o establece la devolución de llamada de advertencia.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crear una devolución de llamada de advertencia personalizada
            IWarningCallback warningCallback = new CustomWarningCallback();

            // Inicializar opciones de carga con devolución de llamada de advertencia
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // Cargar libro de trabajo con opciones
            Workbook workbook = new Workbook("example.xlsx", options);

            // Demostrar el uso de la devolución de llamada de advertencia accediendo a una celda
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


