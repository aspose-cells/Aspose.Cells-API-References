---
title: "Range.AddHyperlink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Agrega un hipervínculo a una celda especificada o a un rango de celdas."
type: docs
url: /es/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Agrega un hipervínculo a una celda especificada o a un rango de celdas.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| address | String | Dirección del hipervínculo. |
| textToDisplay | String | El texto que se mostrará para el hipervínculo especificado. |
| screenTip | String | El texto screenTip para el hipervínculo especificado. |

### Valor de retorno

[`Hyperlink`](../../hyperlink/) object.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // Agregar hipervínculo con dirección, texto para mostrar y descripción emergente.
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // Guarda el libro de trabajo
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


