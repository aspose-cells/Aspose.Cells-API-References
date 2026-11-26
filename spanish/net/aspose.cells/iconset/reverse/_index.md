---
title: "IconSet.Reverse"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconSet. Obtener o establecer la bandera que indica si se invierte el orden predeterminado de los iconos en este conjunto de iconos. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Obtener o establecer la bandera que indica si se invierte el orden predeterminado de los íconos en este conjunto de íconos. El valor predeterminado es false.

```csharp
public bool Reverse { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Agregar formato condicional
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // Establecer el rango
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // Crear formato condicional de conjunto de iconos
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // Configurar conjunto de iconos
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // Demostrar la propiedad Reverse
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // Guarda el libro de trabajo
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


