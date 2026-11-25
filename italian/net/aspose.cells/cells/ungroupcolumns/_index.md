---
title: "Cells.UngroupColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Separa le colonne"
type: docs
url: /it/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Separa le colonne dal raggruppamento.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | Il primo indice di colonna da separare. |
| lastIndex | Int32 | L'ultimo indice di colonna da separare. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Raggruppa le colonne prima per dimostrare la separazione
            worksheet.Cells.GroupColumns(0, 2);

            // Separa le colonne (0 a 2)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


