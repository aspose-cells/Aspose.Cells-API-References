---
title: "Clase IconSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.IconSet. Describe la regla de formato condicional IconSet. Esta regla de formato condicional aplica íconos a las celdas según sus valores"
type: docs
url: /es/net/aspose.cells/iconset/
---
## IconSet class

Describe la regla de formato condicional IconSet. Esta regla de formato condicional aplica iconos a las celdas según sus valores.

```csharp
public class IconSet
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Obtener el[`ConditionalFormattingIcon`](../conditionalformattingicon/) de la colección |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | Obtener la instancia de CFValueObjects. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | Indica si el conjunto de íconos es personalizado. El valor predeterminado es false. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Obtener o establecer la bandera que indica si se invierte el orden predeterminado de los íconos en este conjunto de íconos. El valor predeterminado es false. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Obtener o establecer la bandera que indica si se muestran los valores de las celdas a las que se aplica este conjunto de íconos. El valor predeterminado es true. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Obtener o establecer el tipo de conjunto de íconos a mostrar. Establecer el tipo verificará automáticamente si el recuento actual de Cfvos coincide con el nuevo tipo. Si no coincide, los Cfvos antiguos se limpiarán y se agregarán los Cfvos predeterminados. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Establece el rango de formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Agregar condición
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Obtener conjunto de íconos
            IconSet iconSet = cond.IconSet;

            // Establecer tipo de ícono
            iconSet.Type = IconSetType.Arrows3;

            // Establecer propiedades adicionales
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Asignar valores de celda
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Guardando el archivo Excel
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


