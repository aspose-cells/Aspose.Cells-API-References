---
title: "BorderCollection.SetColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método BorderCollection. Establece el Color de todos los bordes en la colección"
type: docs
url: /es/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Establece el Color de todos los bordes en la colección.

```csharp
public void SetColor(Color color)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | Color | Color de los bordes. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con bordes coloreados
            Style style = workbook.CreateStyle();
            
            // Establecer estilos de línea de borde
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Establecer el color del borde a rojo usando el método SetColor
            style.Borders.SetColor(Color.Red);

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // Ajustar automáticamente la columna para una mejor visibilidad
            worksheet.AutoFitColumn(0);

            // Guarda el libro de trabajo
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


