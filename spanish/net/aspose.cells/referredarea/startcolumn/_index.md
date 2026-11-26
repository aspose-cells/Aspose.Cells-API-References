---
title: "ReferredArea.StartColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. La columna inicial del área"
type: docs
url: /es/net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

La columna inicial del área.

```csharp
public int StartColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["C1"].PutValue("Cherry");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);

            // Crear un rango con nombre que haga referencia a B1:C2
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!B1:C2";

            // Obtener el área referida con recalcular establecido en false
            ReferredArea referredArea = name.GetReferredAreas(false)[0];

            // Demostrar la propiedad StartColumn
            Console.WriteLine("Start Column: " + referredArea.StartColumn);
            Console.WriteLine("End Column: " + referredArea.EndColumn);

            // Imprimir valores en el área referida usando StartColumn
            Cells cells = worksheet.Cells;
            for (int row = referredArea.StartRow; row <= referredArea.EndRow; row++)
            {
                for (int col = referredArea.StartColumn; col <= referredArea.EndColumn; col++)
                {
                    Console.WriteLine(cells[row, col].Name + ": " + cells[row, col].Value);
                }
            }
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


