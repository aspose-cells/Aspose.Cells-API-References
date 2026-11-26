---
title: "Clase GridJsOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridJs.GridJsOptions. Representa todas las opciones de carga para GridJs"
type: docs
url: /es/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

Representa todas las opciones de carga para GridJs

```csharp
public class GridJsOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | Indica si se debe ajustar automáticamente el ancho de las columnas al cargar el archivo, el valor predeterminado es false. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Indica si se debe ajustar automáticamente la altura de las filas al cargar el archivo, el valor predeterminado es false. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Obtiene/Establece si se debe optimizar automáticamente el rendimiento de carga para una hoja de cálculo con celdas grandes. Ignorará algunos estilos /bordes para reducir el tiempo de carga. El valor predeterminado es true. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | Obtiene/Establece el nombre base de la URL de ruta para el controlador GridJs. El valor predeterminado es GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | Obtiene/Establece las PdfSaveOptions personalizadas para la exportación a PDF. Si se establece, se usarán en lugar de las opciones predeterminadas. El valor predeterminado es null. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Obtiene/Establece la columna máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 15. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Obtiene/Establece la fila máxima predeterminada para una hoja de cálculo vacía. El valor predeterminado es 12. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | Obtiene/Establece si se debe habilitar el renderizado de gráficos del lado del cliente. Si se establece en false, GridJs solo emitirá imágenes/formas de gráficos y no requerirá renderizado del lado del cliente. El valor predeterminado es true. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Obtiene/Establece el directorio de caché para almacenar el archivo de hoja de cálculo. Necesitamos establecerlo en una ruta específica antes de usar GridJs. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Obtiene/Establece las carpetas de fuentes para las fuentes en las imágenes/formas renderizadas |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Obtiene/Establece si se muestra el rango máximo que incluye datos, estilo, celdas combinadas y formas. Si la última fila o columna contiene celdas sin valor ni fórmula pero con estilo personalizado, entonces no mostraremos esa fila/columna cuando este valor sea verdadero. El valor predeterminado es verdadero. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Obtiene/Establece si se admite la edición colaborativa, el valor predeterminado es falso. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Obtiene/Establece si se limita el recuento total de formas/imágenes mostradas en una hoja de cálculo. Si se establece en verdadero, GridJs limitará el recuento total de formas o imágenes mostradas en una hoja a MaxShapeOrImageCount. El valor predeterminado es verdadero. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | Obtiene/Establece si GridJs se ejecuta dentro de un host WebAssembly en el navegador en lugar de un proceso de servidor. Cuando es verdadero, no se utiliza FileCacheDirectory / disco / ruta de subproceso de interrupción, y la caché de archivos debe provenir de CacheImp, porque un host de navegador no tiene disco local. Selecciona rutas de código en tiempo de ejecución, por lo que un Aspose.Cells.GridJs.dll sirve a ambos hosts. El valor predeterminado es falso. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | Obtiene/Establece las opciones de configuración de caché JSON. Controla tanto el comportamiento de la caché en memoria (L1) como en disco (L2) para el JSON del libro generado. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Obtiene/Establece si se carga solo la hoja de cálculo activa, el valor predeterminado es falso. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Obtiene/Establece los segundos máximos de tiempo de espera al guardar en PDF. El valor predeterminado es 10. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Obtiene/Establece el recuento total de formas o imágenes mostradas en la hoja activa, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 100. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Obtiene/Establece el ancho o alto máximo para una forma o una imagen, GridJs ignorará la forma o imagen cuyo ancho o alto sea mayor que este valor, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 10000. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Obtiene/Establece el recuento total de formas o imágenes mostradas en el libro, tiene efecto cuando IslimitShapeOrImage=true. El valor predeterminado es 300. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Obtiene/Establece los destinos websocket con prefijo "/topic". El valor predeterminado es "/topic/opr". Se usa solo en modo colaborativo. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Obtiene/Establece el directorio de caché para imágenes. (esto tiene efecto cuando GridJsWorkbook.CacheImp es nulo) La ruta predeterminada será "_piccache" dentro de FileCacheDirectory. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Obtiene/Establece si se verifica si las imágenes tienen la misma fuente, el valor predeterminado es verdadero. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Obtiene/Establece si se guarda el archivo HTML como archivo zip, el valor predeterminado es falso. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Obtiene/Establece si se muestra la hoja de gráfico. El valor predeterminado es falso. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Obtiene/Establece si se omiten las formas que son invisibles para la UI, el valor predeterminado es verdadero. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Obtiene/Establece si se usa PageSetup.PrintArea para el rango de visualización de la UI cuando la hoja tiene la configuración PageSetup para PrintArea. El valor predeterminado es falso. |

## Campos

| Nombre | Descripción |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Implementación personalizada para el almacenamiento en caché. Si deseas almacenar la caché de forma de flujo, debes configurarla e implementarla. Un host WebAssembly (IsWasm = true) debe configurarla, porque no hay disco local para la caché de archivos predeterminada. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | Indica si se usa un id generado por el cliente en lugar del id real de la forma en operaciones relacionadas con la redacción |

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


