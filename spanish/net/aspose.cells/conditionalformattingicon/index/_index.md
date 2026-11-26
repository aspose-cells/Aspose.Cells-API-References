---
title: "ConditionalFormattingIcon.Index"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingIcon. Obtiene y establece el índice de los íconos en el conjunto de íconos"
type: docs
url: /es/net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

Obtiene y establece el índice del ícono en el conjunto de íconos.

```csharp
public int Index { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional de conjunto de iconos
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.IconSet);
            
            // Establecer propiedades del conjunto de iconos
            FormatCondition condition = fcc[0];
            condition.IconSet.Type = IconSetType.Arrows3;
            ConditionalFormattingIconCollection icons = condition.IconSet.CfIcons;

            // Mostrar el índice de cada ícono
            Console.WriteLine("Icon Indexes:");
            for (int i = 0; i < icons.Count; i++)
            {
                Console.WriteLine($"Icon {i}: Index = {icons[i].Index}");
            }

            // Modificar y mostrar la propiedad de índice
            icons[1].Index = 2;
            Console.WriteLine($"Modified Icon 1 Index: {icons[1].Index}");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


