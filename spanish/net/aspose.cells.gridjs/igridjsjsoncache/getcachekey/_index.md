---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IGridJsJsonCache. Generar una clave de caché. Los clientes pueden decidir si incluyen el uid según los requisitos del negocio. Si solo importa el nombre del archivo, ignore el uid y use solo fileName; se recomienda para compartir caché entre el mismo archivo. Si es necesario distinguir archivos con el mismo nombre, use uid en modo estricto"
type: docs
url: /es/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Genera una clave de caché. Los clientes pueden decidir si incluyen el uid según los requisitos del negocio. - Si solo importa el nombre del archivo: ignora el uid y usa solo fileName (recomendado, permite compartir la caché entre el mismo archivo). - Si es necesario distinguir archivos con el mismo nombre: usa uid (modo estricto).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | String | Identificador único del archivo (puede variar por carga) |
| fileName | String | Nombre de archivo original |

### Valor de retorno

Clave de caché

### Ver también

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


