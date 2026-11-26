---
title: "Enum ErrorCellValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.ErrorCellValueType. Representa un valor de celda que contiene un error"
type: docs
url: /es/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Representa un valor de celda que contiene un error.

```csharp
public enum ErrorCellValueType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Value | `1` | Representa el valor de una celda que contiene un error #VALUE!. |
| Ref | `3` | Representa el valor de una celda que contiene un error #REF!. |
| Name | `4` | Representa el valor de una celda que contiene un error #NAME?. |
| NA | `6` | Representa el valor de una celda que contiene un error #N/A. |
| Blocked | `10` | Representa el valor de una celda que contiene un error #BLOCKED!. |
| Busy | `14` | Representa el valor de una celda que contiene un error #BUSY!. |
| Calc | `13` | Representa el valor de una celda que contiene un error #CALC!. |
| Connect | `9` | Representa el valor de una celda que contiene un error #CONNECT!. |
| Field | `12` | Representa el valor de una celda que contiene un error #FIELD!. |
| Spill | `8` | Representa el valor de una celda que contiene un error #SPILL!. |
| Unknown | `11` | Representa el valor de una celda que contiene un error #UNKNOWN!. |
| TimeOut | `19` | Representa el valor de una celda que contiene un error #TIMEOUT!. |
| External | `18` | Representa el valor de una celda que contiene un error #EXTERNAL!. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establece una fórmula que resultará en un error de desbordamiento
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // Calcula fórmulas para desencadenar el error
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Error de desbordamiento esperado
            }
            
            // Obtén el valor enriquecido de la celda
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Verifica el tipo de error
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


