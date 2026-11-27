---
title: "Workbook.CreateBuiltinStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Skapar inbyggd stil med given typ"
type: docs
url: /sv/net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

Skapar inbyggd stil enligt given typ.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | BuiltinStyleType | Den inbyggda stiltypen. |

### Returvärde

[`Style`](../../style/) object

### Exempel

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
            
            // Applicera Good inbyggd stil
            workbook.Worksheets[0].Cells["A1"].PutValue("Good");
            Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
            workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
            
            // Applicera Neutral inbyggd stil
            workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
            Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
            workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
            
            // Spara arbetsboken
            workbook.Save("BuiltinStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


