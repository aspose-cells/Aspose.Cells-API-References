---
title: "Cells.ApplyStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Aplica formatos a toda la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Aplica formatos a toda la hoja de cálculo.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El objeto de estilo que se aplicará. |
| bandera | StyleFlag | Banderas que indican las propiedades de formato aplicadas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            
            // Crear un estilo y establecer el ajuste de texto
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // Crear bandera de estilo y habilitar la bandera de ajuste de texto
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Aplicar el estilo a todas las celdas de la hoja de cálculo
            sheet.Cells.ApplyStyle(style, flag);
            
            // Guarda el libro de trabajo
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


