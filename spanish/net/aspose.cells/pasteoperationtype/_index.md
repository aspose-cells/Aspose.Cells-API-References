---
title: "Enum PasteOperationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.PasteOperationType. Representa el tipo de operación al pegar un rango"
type: docs
url: /es/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Representa el tipo de operación al pegar un rango.

```csharp
public enum PasteOperationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin operación. |
| Add | `1` | Agregar |
| Subtract | `2` | Restar |
| Multiply | `3` | Multiplicar |
| Divide | `4` | Dividir |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // Crear opciones de pegado con PasteOperationType.None
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // Crear rango y copiar con opciones de pegado
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // Guarda el libro de trabajo
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


