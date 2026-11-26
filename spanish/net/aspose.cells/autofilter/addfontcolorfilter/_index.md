---
title: "AutoFilter.AddFontColorFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Añade un filtro de color de fuente"
type: docs
url: /es/net/aspose.cells/autofilter/addfontcolorfilter/
---
## AutoFilter.AddFontColorFilter method

Añade un filtro de color de fuente.

```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| color | CellsColor | El objeto [`CellsColor`](../../cellscolor/). |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFontColorFilterWithInt32CellsColorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra con diferentes colores de fuente
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Item 1");
            cells["A3"].PutValue("Item 2");
            cells["A4"].PutValue("Item 3");
            
            // Establecer colores de fuente
            Style style = cells["A2"].GetStyle();
            style.Font.Color = Color.Red;
            cells["A2"].SetStyle(style);
            
            style = cells["A3"].GetStyle();
            style.Font.Color = Color.Blue;
            cells["A3"].SetStyle(style);
            
            style = cells["A4"].GetStyle();
            style.Font.Color = Color.Green;
            cells["A4"].SetStyle(style);

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Crear filtro de color para fuente roja
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            
            // Agregar filtro de color de fuente
            filter.AddFontColorFilter(0, cr);
            filter.Refresh();
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFilterFontColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


