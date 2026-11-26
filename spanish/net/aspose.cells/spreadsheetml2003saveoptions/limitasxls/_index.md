---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SpreadsheetML2003SaveOptions. Limitar como xls, el índice máximo de fila es 65535 y el índice máximo de columna es 255"
type: docs
url: /es/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

Límite como xls, el índice máximo de fila es 65535 y el índice máximo de columna es 255.

```csharp
public bool LimitAsXls { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Acceder a celdas y crear un rango
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // Guardar con LimitAsXls = true
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // Guardar como SpreadsheetML con límites XLS
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### Ver también

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


