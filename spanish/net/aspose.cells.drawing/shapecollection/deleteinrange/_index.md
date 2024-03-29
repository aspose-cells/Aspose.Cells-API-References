---
title: DeleteInRange
second_title: Referencia de API de Aspose.Cells para .NET
description: Eliminar formas en el rango. Las formas de comentarios no se eliminarán.
type: docs
weight: 390
url: /es/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Eliminar formas en el rango. Las formas de comentarios no se eliminarán.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango. Si las formas están contenidas en el rango, se eliminarán. |

### Ejemplos

```csharp

[C#]
//añadir primera forma
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//añadir segunda forma
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

CellArea area3 = new CellArea();
area3.StartColumn = 0;
area3.StartRow = 5;
area3.EndColumn = 5;
area3.EndRow = 8;

//borrar
shapes.DeleteInRange(area3);
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea)
* class [ShapeCollection](../../shapecollection)
* espacio de nombres [Aspose.Cells.Drawing](../../shapecollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
