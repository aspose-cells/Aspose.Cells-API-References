---
title: "Clase JsonCacheOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridJs.JsonCacheOptions. Opciones de configuración para la caché JSON en GridJs. Controla tanto la caché en memoria L1 como en disco L2."
type: docs
url: /es/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

Opciones de configuración para el almacenamiento en caché JSON en GridJs. Controla el comportamiento de la caché tanto en memoria (L1) como en disco (L2).

```csharp
public class JsonCacheOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | Obtiene/Establece si comprimir la caché en disco usando Gzip (valor predeterminado: true). Tiene efecto cuando Enable = true y se usa la caché predeterminada. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | Obtiene/Establece la ruta del directorio de la caché en disco. Tiene efecto cuando Enable = true y se usa la caché predeterminada. Predeterminado: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | Obtiene/Establece el TTL para la caché en disco (valor predeterminado: 24 horas). Tiene efecto cuando Enable = true y se usa la caché predeterminada. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | Obtiene/Establece si habilitar la caché JSON para una respuesta más rápida. Cuando está habilitado, GridJs almacenará en caché el JSON generado y lo reutilizará en solicitudes posteriores. El valor predeterminado es false. Nota: Necesita establecer Implementation para usar un almacenamiento de caché personalizado. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | Obtiene/Establece si habilitar la caché en disco (valor predeterminado: true). Tiene efecto cuando Enable = true y se usa la caché predeterminada. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | Obtiene/Establece la implementación personalizada de la caché JSON. Si no se establece, GridJs usará la caché predeterminada de memoria + disco. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | Obtiene/Establece el tamaño máximo de la caché en disco en MB (valor predeterminado: 500 MB). Tiene efecto cuando Enable = true y se usa la caché predeterminada. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | Obtiene/Establece el número máximo de entradas en la caché de memoria (valor predeterminado: 1000). Tiene efecto cuando Enable = true y se usa la caché predeterminada. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | Obtiene/Establece el TTL para la caché de memoria (valor predeterminado: 1 hora). Tiene efecto cuando Enable = true y se usa la caché predeterminada. |

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


