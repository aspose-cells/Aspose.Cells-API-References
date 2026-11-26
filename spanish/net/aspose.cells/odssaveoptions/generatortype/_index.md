---
title: "OdsSaveOptions.GeneratorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsSaveOptions. Obtiene y establece el generador del archivo ods"
type: docs
url: /es/net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

Obtiene y establece el generador del archivo ods.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyGeneratorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Crear y configurar las opciones de guardado ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions
            {
                GeneratorType = OdsGeneratorType.LibreOffice,
                IsStrictSchema11 = true
            };

            // Guardar el libro de trabajo con las opciones especificadas
            workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Ver también

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


