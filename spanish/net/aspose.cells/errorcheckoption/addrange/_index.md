---
title: "ErrorCheckOption.AddRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ErrorCheckOption method. Agrega un rango influenciado por esta configuración"
type: docs
url: /es/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Añade un rango influenciado por esta configuración.

```csharp
public int AddRange(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | el rango a agregar. |

### Valor de retorno

el índice del rango agregado en la lista de rangos de esta configuración.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // Agregar rangos usando CellArea
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // Guarda el libro de trabajo
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


