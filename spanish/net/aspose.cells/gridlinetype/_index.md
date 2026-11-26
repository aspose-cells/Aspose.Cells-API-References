---
title: "Enumeración GridlineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridlineType enum. Enumera los tipos de líneas de cuadrícula"
type: docs
url: /es/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Enumera el tipo de línea de cuadrícula.

```csharp
public enum GridlineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Dotted | `0` | Representa una línea punteada. |
| Hair | `1` | Representa una línea delgada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear opciones de guardado y establecer el tipo de línea de cuadrícula
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // Agregar algunos datos de ejemplo para ver las líneas de cuadrícula
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // Guardar el libro de trabajo con las opciones de guardado
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


