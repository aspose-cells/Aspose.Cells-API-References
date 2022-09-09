---
title: Remove
second_title: Referencia de API de Aspose.Cells para .NET
description: Eliminar la forma.
type: docs
weight: 420
url: /es/net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Eliminar la forma.

```csharp
public void Remove(Shape shape)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| shape | Shape |  |

### Ejemplos

```csharp

[C#]
//añadir primera forma
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//añadir segunda forma
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

// obtener la forma
Shape s = shapes["Rectangle 1"];// o formas[0];
if (s != null)
{
    //retirar 
    shapes.Remove(s);
}
```

### Ver también

* class [Shape](../../shape)
* class [ShapeCollection](../../shapecollection)
* espacio de nombres [Aspose.Cells.Drawing](../../shapecollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->