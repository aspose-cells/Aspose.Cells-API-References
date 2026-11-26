---
title: "Cell.SharedStyleIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el índice de estilo compartido de la celda en el pool de estilos"
type: docs
url: /es/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Obtiene el índice de estilo compartido de la celda en el pool de estilos.

```csharp
public int SharedStyleIndex { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un estilo y establece algunas propiedades
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // Aplicar el estilo a la celda A1
            worksheet.Cells["A1"].SetStyle(style);

            // Obtén el índice de estilo compartido de la celda A1
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // Recupera el estilo del pool de estilos usando el índice
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // Muestra la información del estilo para verificar
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


