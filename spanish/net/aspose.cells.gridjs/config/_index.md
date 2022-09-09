---
title: Config
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa todas las configuraciones para GridJs
type: docs
weight: 10
url: /es/net/aspose.cells.gridjs/config/
---
## Config class

Representa todas las configuraciones para GridJs

```csharp
public class Config
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Config](config)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells) { get; set; } |  |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol) { get; set; } | Establece/Obtiene la columna máxima predeterminada para una hoja de trabajo vacía |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow) { get; set; } | Establece la fila máxima predeterminada para una hoja de trabajo vacía |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory) { get; set; } | Establece/Obtiene el directorio de caché para el archivo del libro de trabajo |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent) { get; set; } | Establece si mostrar el rango máximo que incluye datos, estilo, celdas combinadas y formas. el valor predeterminado es verdadero. Si la última fila o columna contiene celdas sin valor y fórmula pero tiene un estilo personalizado entonces no mostraremos esto fila/columna cuando este valor es true |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage) { get; set; } | Establece si se limita el recuento total de formas/imágenes de visualización dentro de una hoja de trabajo; si se establece en verdadero, GridJs limitará el tamaño total de forma/imagen de visualización dentro de una hoja de trabajo a MaxShapeOrImageCount el valor predeterminado es true |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds) { get; set; } | Establece/obtiene los segundos máximos de tiempo de espera cuando se guarda en pdf |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount) { get; set; } | Establece/Obtiene el recuento total de formas/imágenes de visualización dentro de la hoja activa, tendrá efecto cuando IslimitShapes=true |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight) { get; set; } | Establece/Obtiene el ancho o alto máximo para una forma/imagen, GridJs ignorará la forma/imagen con un ancho o alto mayor que esto, tendrá efecto cuando IslimitShapes=true |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount) { get; set; } | Establece/Obtiene el recuento total de formas/imágenes de visualización dentro de todo el libro de trabajo, tendrá efecto cuando IslimitShapes=true |
| static [PageSize](../../aspose.cells.gridjs/config/pagesize) { get; set; } | Establece si se debe realizar la paginación GridJs limitará el tamaño de la fila según el tamaño de la página, si el tamaño de la página es -1, no realizará la paginación el valor predeterminado es -1 |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory) { get; set; } | Establece/Obtiene el directorio de caché para imágenes |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting) { get; set; } | Establece si se debe verificar si la imagen tiene la misma fuente, el valor predeterminado es true el valor predeterminado es true |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip) { get; set; } | Establece si guardar el archivo html como archivo zip, el valor predeterminado es false el valor predeterminado es true |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder)(string, bool) | Establece la carpeta de fuentes |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders)(string[], bool) | Establece las carpetas de fuentes |

### Ver también

* espacio de nombres [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* asamblea [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->