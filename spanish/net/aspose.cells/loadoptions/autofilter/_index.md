---
title: "LoadOptions.AutoFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Indica si se filtra automáticamente los datos al cargar los archivos"
type: docs
url: /es/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Indica si se filtra automáticamente los datos al cargar los archivos.

```csharp
public bool AutoFilter { get; set; }
```

### Observaciones

A veces, aunque el autofiltro está configurado, las filas correspondientes no se ocultan en el archivo. Ahora solo funciona para archivos SpreadSheetML.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Crear opciones de carga y habilitar AutoFilter
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // Cargar libro de trabajo con AutoFilter habilitado
            Workbook workbook = new Workbook("example.xlsx", options);

            // Acceder a la primera hoja de cálculo y aplicar AutoFilter
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


