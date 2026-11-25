---
title: "AutoFilter.DynamicFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Aggiunge un filtro dinamico"
type: docs
url: /it/net/aspose.cells/autofilter/dynamicfilter/
---
## AutoFilter.DynamicFilter method

Aggiunge un filtro dinamico.

```csharp
public void DynamicFilter(int fieldIndex, DynamicFilterType dynamicFilterType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| dynamicFilterType | DynamicFilterType | Tipo di filtro dinamico. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodDynamicFilterWithInt32DynamicFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            // Applica il filtro automatico usando la firma del metodo corretta
            worksheet.AutoFilter.Range = "A1:A6";

            // Applica filtro dinamico per le date di marzo
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            workbook.Save("DynamicFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


