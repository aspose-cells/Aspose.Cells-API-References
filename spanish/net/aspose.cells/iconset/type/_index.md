---
title: "IconSet.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconSet. Obtener o establecer el tipo de conjunto de iconos a mostrar. Al establecer el tipo se verificará automáticamente si el recuento actual de Cfvoss coincide con el nuevo tipo. Si no coincide, los Cfvos antiguos se limpiarán y se agregarán los Cfvos predeterminados."
type: docs
url: /es/net/aspose.cells/iconset/type/
---
## IconSet.Type property

Obtener o establecer el tipo de conjunto de íconos a mostrar. Establecer el tipo verificará automáticamente si el recuento actual de Cfvos coincide con el nuevo tipo. Si no coincide, los Cfvos antiguos se limpiarán y se agregarán los Cfvos predeterminados.

```csharp
public IconSetType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];
            IconSet iconSet = cond.IconSet;

            // Demostrar el uso de la propiedad Type
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### Ver también

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


