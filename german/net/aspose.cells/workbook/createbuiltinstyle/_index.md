---
title: "Workbook.CreateBuiltinStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Erstellt einen integrierten Stil vom angegebenen Typ"
type: docs
url: /de/net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

Erstellt einen integrierten Stil anhand des angegebenen Typs.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | BuiltinStyleType | Der integrierte Stiltyp. |

### Rückgabewert

[`Style`](../../style/) object

### Beispiele

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
            
            // Guten integrierten Stil anwenden
            workbook.Worksheets[0].Cells["A1"].PutValue("Good");
            Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
            workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
            
            // Neutralen integrierten Stil anwenden
            workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
            Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
            workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
            
            // Speichere die Arbeitsmappe
            workbook.Save("BuiltinStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


