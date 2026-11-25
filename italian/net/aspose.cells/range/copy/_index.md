---
title: "Range.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Copia l'intervallo con le opzioni Incolla speciale"
type: docs
url: /it/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Copia l'intervallo con le opzioni incolla speciale.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo di origine. |
| opzioni | PasteOptions | Le opzioni Incolla speciale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangePasteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea dati di esempio nell'intervallo di origine
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crea intervalli con tipo completamente qualificato
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // Imposta le opzioni di incolla
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // Copia con le opzioni di incolla
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Copia i dati (incluse le formule), la formattazione, gli oggetti di disegno ecc. da un intervallo di origine.

```csharp
public void Copy(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| range | Range | Oggetto [`Range`](../) di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Crea intervalli di origine e di destinazione
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // Riempire l'intervallo di origine con dati di esempio
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // Copia l'intervallo di origine nella destinazione
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


