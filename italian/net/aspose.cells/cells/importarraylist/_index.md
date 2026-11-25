---
title: "Cells.ImportArrayList"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa una ArrayList di dati in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Importa un arraylist di dati in un foglio di lavoro.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayList | ArrayList | ArrayList di dati. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| isVertical | Booleano | Specifica se importare i dati verticalmente o orizzontalmente. |

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportArrayListWithArrayListInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ArrayList data = new ArrayList();
            data.Add("Name");
            data.Add("Age");
            data.Add("City");
            
            cells.ImportArrayList(data, 0, 0, false);
            
            data.Clear();
            data.Add("John");
            data.Add(30);
            data.Add("New York");
            
            cells.ImportArrayList(data, 1, 0, false);
            
            workbook.Save("ImportArrayListDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


