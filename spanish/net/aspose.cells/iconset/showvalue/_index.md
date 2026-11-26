---
title: "IconSet.ShowValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconSet. Obtener o establecer la bandera que indica si se deben mostrar los valores de las celdas a las que se aplica este conjunto de iconos. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

Obtener o establecer la bandera que indica si se muestran los valores de las celdas a las que se aplica este conjunto de íconos. El valor predeterminado es true.

```csharp
public bool ShowValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyShowValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);
            sheet.Cells["A5"].PutValue(50);

            // Agregar formato condicional de conjunto de iconos
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            int index = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[index];

            // Establecer propiedades del conjunto de iconos
            condition.IconSet.Type = IconSetType.TrafficLights31;
            condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
            condition.IconSet.Reverse = false;

            // Establecer el rango para el formato condicional
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            formatConditions.AddArea(area);

            // Guarda el libro de trabajo
            workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
        }
    }
}
```

### Ver también

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


