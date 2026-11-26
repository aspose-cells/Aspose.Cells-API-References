---
title: "Cells.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene el elemento Cell en el índice de fila y columna de celda especificados"
type: docs
url: /es/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Obtiene el elemento [`Cell`](../../cell/) en el índice de fila y columna de celda especificados.

```csharp
public Cell this[int row, int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | Índice de fila. |
| columna | Índice de columna. |

### Valor de retorno

El objeto [`Cell`](../../cell/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Usando la propiedad Item para acceder y modificar celdas
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // Usando la propiedad Style a través de Cells
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // Guarda el libro de trabajo
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Obtiene el elemento [`Cell`](../../cell/) con el nombre de celda especificado.

```csharp
public Cell this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | Nombre de la celda, incluyendo su letra de columna y número de fila, por ejemplo A5. |

### Valor de retorno

Un objeto [`Cell`](../../cell/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la colección de celdas
            Cells cells = worksheet.Cells;
            
            // Establecer valores usando la propiedad Item
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // Establecer valores en un rango usando la propiedad Item
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // Acceder y modificar propiedades de la celda usando Item
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


