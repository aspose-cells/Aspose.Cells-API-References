---
title: "ShapeCollection.AddFreeform"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade una forma libre a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Agrega una forma libre a la hoja de cálculo.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de la forma libre desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal de la forma libre desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura de la forma libre, en unidades de píxel. |
| ancho | Int32 | Representa el ancho de la forma libre, en unidades de píxel. |
| rutas | ShapePath[] | Representa una ruta definida por el usuario |

### Valor de retorno

Una forma libre.

### Observaciones

Aviso: que el ancho y la altura en los parámetros pueden ser cualquier valor entero positivo, no el ancho y la altura total del arreglo ShapePath especificado por ’paths'. La relación entre ellos es una relación de escala‑relleno, es decir, cada objeto ShapePath se escalará según el ancho y la altura. Por lo tanto, cuando hay varios objetos en 'paths', cada objeto ShapePath debe diseñarse razonablemente para cumplir con las expectativas. Cuando solo hay un objeto ShapePath y no existen otros requisitos, pasar el ancho y la altura del objeto como valores de parámetro es una buena solución.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Crear rutas de figuras personalizadas
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // Añadir forma libre a la hoja de cálculo
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // Guarda el libro de trabajo
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


