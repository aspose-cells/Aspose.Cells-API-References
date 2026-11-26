---
title: "SmartTagCollection.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagCollection. Obtiene la columna de las etiquetas inteligentes de la celda"
type: docs
url: /es/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

Obtiene la columna de las smart tags de la celda.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade una etiqueta inteligente a la celda C5 (fila 4, columna 2)
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // Obtén la SmartTagCollection para la celda C5
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Muestra la columna de la celda que contiene estas etiquetas inteligentes
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // Añade otra etiqueta inteligente a la celda E2 (fila 1, columna 4) para demostrar una columna diferente
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


