---
title: "Range.AutoFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Riempie automaticamente l'intervallo di destinazione"
type: docs
url: /it/net/aspose.cells/range/autofill/
---
## AutoFill(Range) {#autofill}

Riempie automaticamente l'intervallo di destinazione.

```csharp
public void AutoFill(Range target)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Intervallo | l'intervallo di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAutoFillWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            
            Aspose.Cells.Range source = cells.CreateRange("A1:A2");
            Aspose.Cells.Range target = cells.CreateRange("A3:A10");
            
            source.AutoFill(target);
            
            workbook.Save("AutoFillWithRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFill(Range, AutoFillType) {#autofill_1}

Riempie automaticamente l'intervallo di destinazione.

```csharp
public void AutoFill(Range target, AutoFillType autoFillType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | Intervallo | L'intervallo di destinazione. |
| autoFillType | AutoFillType | Il tipo di riempimento automatico. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAutoFillWithRangeAutoFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A5");
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B5");
            sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Verifica il risultato stampando i valori
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Target cell B{i+1} value: {targetRange[i, 0].IntValue}");
            }
        }
    }
}
```

### Vedi anche

* enum [AutoFillType](../../autofilltype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


