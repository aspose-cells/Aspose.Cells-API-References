---
title: "Cells.ApplyStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Applica formati a un intero foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Applica formati a un intero foglio di lavoro.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | L'oggetto stile che verrà applicato. |
| flag | StyleFlag | Flag che indicano le proprietà di formattazione applicate. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea uno stile e imposta l'andare a capo del testo
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // Crea flag di stile e abilita il flag di ritorno a capo del testo
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Applica lo stile a tutte le celle del foglio di lavoro
            sheet.Cells.ApplyStyle(style, flag);
            
            // Salva la cartella di lavoro
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


