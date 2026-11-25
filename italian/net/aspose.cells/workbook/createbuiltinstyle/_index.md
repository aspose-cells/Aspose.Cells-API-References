---
title: "Workbook.CreateBuiltinStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Crea uno stile incorporato del tipo specificato"
type: docs
url: /it/net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

Crea uno stile predefinito del tipo specificato.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | BuiltinStyleType | Lo stile incorporato. |

### Valore di ritorno

[`Style`](../../style/) object

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateBuiltinStyleWithBuiltinStyleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Applica lo stile incorporato Good
            workbook.Worksheets[0].Cells["A1"].PutValue("Good");
            Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
            workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
            
            // Applica lo stile incorporato Neutral
            workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
            Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
            workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
            
            // Salva la cartella di lavoro
            workbook.Save("BuiltinStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


