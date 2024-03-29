---
title: MultiThreadReading
second_title: Referencia de API de Aspose.Cells para .NET
description: Obtiene o establece si el modelo de datos de celdas debe admitir la lectura de subprocesos múltiples. El valor predeterminado de esta propiedad es falso.
type: docs
weight: 200
url: /es/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Obtiene o establece si el modelo de datos de celdas debe admitir la lectura de subprocesos múltiples. El valor predeterminado de esta propiedad es falso.

```csharp
public bool MultiThreadReading { get; set; }
```

### Observaciones

Si hay varios subprocesos para leer objetos Fila/Celda en esta colección al mismo tiempo, esta propiedad debe establecerse como verdadera; de lo contrario, se pueden producir resultados inesperados. esta colección. Tenga en cuenta que algunas funciones no admiten la lectura de subprocesos múltiples, como valores de formato (por[`StringValue`](../../cell/stringvalue) ,[`DisplayStringValue`](../../cell/displaystringvalue) .etc.). Entonces, incluso con esta propiedad configurada como verdadera, esas API aún pueden dar resultados inesperados para la lectura de subprocesos múltiples.

### Ver también

* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
