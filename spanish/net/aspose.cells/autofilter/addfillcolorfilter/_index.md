---
title: "AutoFilter.AddFillColorFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Añade un filtro de color de relleno"
type: docs
url: /es/net/aspose.cells/autofilter/addfillcolorfilter/
---
## AutoFilter.AddFillColorFilter method

Añade un filtro de color de relleno.

```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor, 
    CellsColor backgroundColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| patrón | BackgroundType | El tipo de patrón de fondo. |
| foregroundColor | CellsColor | El color de primer plano. |
| backgroundColor | CellsColor | El color de fondo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFillColorFilterWithInt32BackgroundTypeCellsColorCDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra con diferentes colores de relleno
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");
            
            // Aplicar diferentes colores de relleno
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);
            
            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);
            
            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Cree filtro automático
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Crear color de celdas para filtrado
            CellsColor filterColor = workbook.CreateCellsColor();
            filterColor.Color = Color.Red;
            
            // Aplicar filtro de color de relleno
            filter.AddFillColorFilter(0, BackgroundType.Solid, filterColor, filterColor);
            filter.Refresh();
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFilterFillColorDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


