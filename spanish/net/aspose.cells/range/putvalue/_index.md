---
title: "Range.PutValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Inserta un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de las celdas se restablecerá"
type: docs
url: /es/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Inserta un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y se restablecerá el formato numérico de la celda.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | String | Valor de entrada |
| isConverted | Booleano | True: convertido a otro tipo de datos si es apropiado. |
| setStyle | Booleano | True: establecer el formato numérico al estilo de la celda al convertir a otro tipo de datos |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            
            Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


