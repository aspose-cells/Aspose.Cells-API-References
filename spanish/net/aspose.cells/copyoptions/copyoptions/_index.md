---
title: "CopyOptions.CopyOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de CopyOptions. Constructor de CopyOptions"
type: docs
url: /es/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

Constructor de CopyOptions.

```csharp
public CopyOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregue una hoja y obtenga la primera hoja
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // Agregue datos de muestra a la hoja de origen
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // Cree CopyOptions usando el constructor
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // Copie filas con las opciones
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // Guarda el libro de trabajo
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


