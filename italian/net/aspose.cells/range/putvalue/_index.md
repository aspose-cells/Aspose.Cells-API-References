---
title: "Range.PutValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Inserisce un valore nell'intervallo; se appropriato il valore verrà convertito in un altro tipo di dato e il formato numerico delle celle verrà ripristinato"
type: docs
url: /it/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Inserisce un valore nell'intervallo; se opportuno il valore sarà convertito in un altro tipo di dati e il formato numerico della cella verrà ripristinato.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | String | Valore di input |
| isConverted | Booleano | True: convertito in un altro tipo di dato se appropriato. |
| setStyle | Booleano | True: imposta il formato numerico nello stile della cella quando si converte in un altro tipo di dato |

### Esempi

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

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


