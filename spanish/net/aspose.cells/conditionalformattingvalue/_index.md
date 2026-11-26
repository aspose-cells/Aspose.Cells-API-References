---
title: "Clase ConditionalFormattingValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ConditionalFormattingValue. Describe los valores de los puntos de interpolación en una barra de datos de escala de degradado o iconSet"
type: docs
url: /es/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

Describe los valores de los puntos de interpolación en una escala de degradado, barra de datos o conjunto de íconos.

```csharp
public class ConditionalFormattingValue
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Obtenga o establezca la bandera Greater Than Or Equal. Úsela solo para conjuntos de iconos, determina si este valor de umbral utiliza el operador mayor o igual que. 'false' indica que se usa 'greater than' en lugar de 'greater than or equal to'. El valor predeterminado es true. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Obtenga o establezca el tipo de este objeto de valor de formato condicional. Establecer el tipo a FormatConditionValueType.Min o FormatConditionValueType.Max establecerá automáticamente \"Value\" a null. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Obtenga o establezca el valor de este objeto de valor de formato condicional. Debe usarse junto con Type. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establece el rango de formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Agregar condición
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Configurando propiedades para ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Estableciendo valor mínimo
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Estableciendo valor medio
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Estableciendo valor máximo
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


