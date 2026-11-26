---
title: "Interfaz IGridJsJsonCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridJs.IGridJsJsonCache interfaz. Interfaz de caché JSON que los clientes implementan para estrategias específicas de almacenamiento e invalidación."
type: docs
url: /es/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

Interfaz de caché JSON - los clientes implementan estrategias específicas de almacenamiento e invalidación

```csharp
public interface IGridJsJsonCache
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Borrar todas las cachés |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Genera una clave de caché. Los clientes pueden decidir si incluyen el uid según los requisitos del negocio. - Si solo importa el nombre del archivo: ignora el uid y usa solo fileName (recomendado, permite compartir la caché entre el mismo archivo). - Si es necesario distinguir archivos con el mismo nombre: usa uid (modo estricto). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Invalidar la entrada de caché especificada. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Invalidar todas las entradas de caché que contengan el uid especificado. Esto es útil cuando no conoces el fileName exacto utilizado para la caché. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | Escribir JSON en la caché. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | Intentar recuperar JSON de la caché. |

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


