---
title: "SmartTagCollection.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagCollection. Obtiene la fila de las etiquetas inteligentes de la celda"
type: docs
url: /es/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

Obtiene la fila de las smart tags de la celda.

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade una etiqueta inteligente a la celda A1 (fila 0, columna 0)
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // Obtén la SmartTagCollection para la celda A1
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Muestra la fila de la celda que contiene estas etiquetas inteligentes
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // Nota: La propiedad Row es de solo lectura, por lo que no podemos establecerla
            // smartTags.Row = 5; // Esto causaría un error de compilación

            // Añade otra etiqueta inteligente a la celda B3 (fila 2, columna 1) para demostrar una fila diferente
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


