---
title: "DataBar.Direction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtiene o establece la dirección en que se muestra la barra de datos"
type: docs
url: /es/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

Obtiene o establece la dirección en que se muestra el databar.

```csharp
public TextDirectionType Direction { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para demostrar barras de datos
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // Agregar formato condicional de barra de datos
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // Definir el área de la celda para la condición de formato
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // Agregar la condición DataBar y obtener la referencia
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // Mostrar el valor actual de Direction
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // Cambiar la dirección a RightToLeft y demostrar
            dataBar.Direction = TextDirectionType.RightToLeft;

            // Configuración adicional para una mejor visualización
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // Guardar el libro de trabajo para mostrar el efecto
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


