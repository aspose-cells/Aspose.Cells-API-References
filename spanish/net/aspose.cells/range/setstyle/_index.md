---
title: "Range.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Aplicar el estilo de celda"
type: docs
url: /es/net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Aplicar el estilo de celda.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El estilo de la celda. |
| explicitFlag | Booleano | True, solo sobrescribiendo el formato que está establecido explícitamente. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
            range.SetStyle(style, true);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Establece el estilo del rango.

```csharp
public void SetStyle(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El objeto Style. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.Font.Color = Color.Red;
            style.Font.Underline = FontUnderlineType.Single;

            // Aplicar el estilo a una celda
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].SetStyle(style);

            // Crear un rango y aplicar el mismo estilo
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
            range.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


