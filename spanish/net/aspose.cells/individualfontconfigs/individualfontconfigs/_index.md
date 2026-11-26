---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de IndividualFontConfigs. Ctor"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

Ctor.

```csharp
public IndividualFontConfigs()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear opciones de carga con IndividualFontConfigs
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // Crear un nuevo libro de trabajo con hoja de cálculo predeterminada
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // Acceder a una hoja de cálculo y agregar texto
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // Guardar el libro de trabajo (las opciones de carga no son necesarias para guardar)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### Ver también

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


