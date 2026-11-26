---
title: "BorderCollection.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método BorderCollection. Establece el estilo de todos los bordes de la colección"
type: docs
url: /es/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Establece el estilo de todos los bordes de la colección.

```csharp
public void SetStyle(CellBorderType style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | CellBorderType | Estilo de los bordes |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la celda C6 y su estilo
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // Establecer el color y el estilo del borde
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // Aplique el estilo a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### Ver también

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


