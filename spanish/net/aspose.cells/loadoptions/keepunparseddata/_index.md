---
title: "LoadOptions.KeepUnparsedData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Indica si se mantiene los datos no analizados en memoria para el libro de trabajo cuando se carga desde el archivo de plantilla. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Indica si se mantiene los datos no analizados en memoria para el Workbook cuando se carga desde un archivo de plantilla. El valor predeterminado es true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Observaciones

Para escenarios en los que el usuario solo necesita leer algunos contenidos del archivo de plantilla y no necesita guardar el libro de trabajo, establecer esta propiedad como false puede mejorar el rendimiento, especialmente cuando se usa junto con algún tipo de LoadFilter,

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // Cree opciones de carga y establezca KeepUnparsedData en false
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // Cargar libro de trabajo con opciones
            Workbook workbook = new Workbook("example.xlsx", options);

            // Acceda a la hoja de cálculo y demuestre que los datos no analizados no se conservan
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

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


