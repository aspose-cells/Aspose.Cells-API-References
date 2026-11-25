---
title: "Cells.IsColumnHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Verifica se una colonna all'indice specificato è nascosta"
type: docs
url: /it/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Verifica se una colonna all'indice specificato è nascosta.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | indice colonna |

### Valore di ritorno

vero se la colonna è nascosta.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Nascondi la colonna C (indice 2)
            cells.HideColumn(2);
            
            // Verifica se la colonna C è nascosta
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


