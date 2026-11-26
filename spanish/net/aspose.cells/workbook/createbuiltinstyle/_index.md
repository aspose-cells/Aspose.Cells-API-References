---
title: "Workbook.CreateBuiltinStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Crea un estilo incorporado según el tipo dado"
type: docs
url: /es/net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

Crea un estilo incorporado según el tipo dado.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | BuiltinStyleType | El estilo incorporado. |

### Valor de retorno

[`Style`](../../style/) object

### Ejemplos

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
            
            // Aplicar estilo incorporado Bueno
            workbook.Worksheets[0].Cells["A1"].PutValue("Good");
            Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
            workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
            
            // Aplicar estilo incorporado Neutral
            workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
            Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
            workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
            
            // Guarda el libro de trabajo
            workbook.Save("BuiltinStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


