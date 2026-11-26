---
title: "CopyOptions.KeepMacros"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CopyOptions. Indica si se mantienen macros"
type: docs
url: /es/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Indica si se conservan las macros;

```csharp
public bool KeepMacros { get; set; }
```

### Observaciones

Solo para copiar el libro de trabajo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo fuente con macros (usando un archivo de plantilla que contiene macros)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            
            // Establecer opciones de copia con KeepMacros true
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // Copiar worksheet con macros
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // Guardar resultado
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


