---
title: "Clase Config"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridJs.Config. Representa todas las configuraciones estáticas para GridJs"
type: docs
url: /es/net/aspose.cells.gridjs/config/
---
## Config class

Representa todas las configuraciones estáticas para GridJs

```csharp
public class Config
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Config](config/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | Indica si se deben ajustar automáticamente los anchos de columna durante la carga del archivo. El valor predeterminado es `false`. Advertencia: Configurar esto a `true` realizará una operación de ajuste automático de todas las columnas después de la carga, lo que puede tener un impacto notable en el rendimiento. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | Indica si se deben ajustar automáticamente las alturas de fila durante la carga del archivo. El valor predeterminado es `false`. Advertencia: Configurar esto a `true` realizará una operación de ajuste automático de todas las filas después de la carga, lo que puede tener un impacto notable en el rendimiento. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Obtiene/Establece si se debe optimizar automáticamente el rendimiento de carga para una hoja de cálculo con celdas grandes. Ignorará algunos estilos /bordes para reducir el tiempo de carga. El valor predeterminado es true. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | Obtiene/establece el nombre de ruta base para la URL del controlador GridJs. El valor predeterminado es "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | Obtiene/Establece las PdfSaveOptions personalizadas para la exportación a PDF. Si se establece, se usarán en lugar de las opciones predeterminadas. El valor predeterminado es null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Obtiene/Establece la columna máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Obtiene/Establece la fila máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 12. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | Obtiene/establece si habilitar la renderización de gráficos del lado del cliente. Si se establece en false, GridJs recurrirá solo a imágenes/formas de gráficos generados por el servidor. El valor predeterminado es true. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Obtiene/Establece el directorio de caché para almacenar el archivo de hoja de cálculo. Necesitamos establecerlo en una ruta específica antes de usar GridJs. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Obtiene/Establece si se muestra el rango máximo que incluye datos, estilo, celdas combinadas y formas. Si la última fila o columna contiene celdas sin valor ni fórmula pero con estilo personalizado, entonces no mostraremos esa fila/columna cuando este valor sea verdadero. El valor predeterminado es verdadero. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Obtiene/Establece si se admite la edición colaborativa, el valor predeterminado es falso. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Obtiene/Establece si se limita el recuento total de formas/imágenes mostradas en una hoja de cálculo. Si se establece en verdadero, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja a MaxShapeOrImageCount. El valor predeterminado es verdadero. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | Obtiene/establece si GridJs se ejecuta dentro de un host WebAssembly del navegador en lugar de un proceso de servidor. Cuando es true, no se utiliza ninguna ruta FileCacheDirectory / disco / hilo de interrupción y la caché de archivos debe provenir de GridJsOptions.CacheImp. GridJsOptions.IsWasm establece esto cuando se construye el servicio GridJs, de modo que un solo Aspose.Cells.GridJs.dll sirve a ambos hosts. El valor predeterminado es false. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | Obtiene/Establece las opciones de configuración de caché JSON. Controla tanto el comportamiento de la caché en memoria (L1) como en disco (L2) para el JSON del libro generado. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Obtiene/Establece si se carga solo la hoja de cálculo activa, el valor predeterminado es falso. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Obtiene/Establece los segundos máximos de tiempo de espera al guardar en PDF. El valor predeterminado es 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Obtiene/Establece el recuento total de formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Obtiene/Establece el ancho o alto máximo para una forma o una imagen, GridJs ignorará la forma o imagen cuyo ancho o alto sea mayor que este valor, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Obtiene/Establece el recuento total de formas o imágenes mostradas en el libro, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Obtiene/Establece los destinos websocket con prefijo "/topic". El valor predeterminado es "/topic/opr". Se usa solo en modo colaborativo. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Obtiene/Establece el directorio de caché para imágenes. (esto tiene efecto cuando GridJsWorkbook.CacheImp es nulo) La ruta predeterminada será "_piccache" dentro de FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Obtiene/Establece si se verifica si las imágenes tienen la misma fuente, el valor predeterminado es verdadero. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Obtiene/Establece si se guarda el archivo HTML como archivo zip, el valor predeterminado es falso. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Obtiene/Establece si se muestra la hoja de gráfico. El valor predeterminado es falso. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Obtiene/Establece si se omiten las formas que son invisibles para la UI, el valor predeterminado es verdadero. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Obtiene/Establece si se usa PageSetup.PrintArea para el rango de visualización de la UI cuando la hoja tiene la configuración PageSetup para PrintArea. El valor predeterminado es falso. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Establece la carpeta de fuentes |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Establece las carpetas de fuentes |

## Campos

| Nombre | Descripción |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | Indica si se usa un id generado por el cliente en lugar del id real de la forma en operaciones relacionadas con la redacción |

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


