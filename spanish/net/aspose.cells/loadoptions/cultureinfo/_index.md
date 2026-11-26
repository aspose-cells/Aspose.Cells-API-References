---
title: "LoadOptions.CultureInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene o establece la configuración regional utilizada para el Workbook que se cargará"
type: docs
url: /es/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Observaciones

Esta propiedad tiene el mismo efecto que [`Region`](../region/) para establecer la configuración regional.

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Crear archivo Excel de ejemplo
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // Cargar con una cultura específica
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


