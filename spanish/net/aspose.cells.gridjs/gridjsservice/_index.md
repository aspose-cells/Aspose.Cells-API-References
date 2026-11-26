---
title: "Clase GridJsService"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridJs.GridJsService class. Proporciona las API básicas de operación utilizadas en acciones del controlador"
type: docs
url: /es/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Proporciona las API básicas de operación utilizadas en acciones de controlador.

```csharp
public class GridJsService : IGridJsService
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | El constructor de GridJsService para hosts que construyen el objeto de opciones ellos mismos (el host WASM del navegador y cualquier configuración de servidor sin DI). |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | El constructor predeterminado de GridJsService |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Representa la configuración del libro de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | Aplica la operación de agregar imagen desde archivo local (los bytes del archivo provienen de JS FormData o cualquier host). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Aplica la operación de agregar imagen desde archivo local. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Aplica la operación de agregar imagen desde URL remota. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Comprueba si la instancia del libro de trabajo está en la caché de memoria. este método se aplica solo para el modo colaborativo. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | Elimina todas las entradas de caché JSON (memoria y disco). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | Elimina todas las entradas de caché JSON que pertenecen al id único especificado. Llame a esto después de modificar el archivo fuente fuera de banda para que la siguiente solicitud regenere el JSON. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Aplica la operación de copiar imagen. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | este método es solo para Java, implementa el método destroy en DisposableBean, que será llamado automáticamente por Spring al finalizar la solicitud; en realidad llamará al método Dispose |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Obtiene la cadena JSON del archivo por el id único especificado. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Obtiene la cadena JSON del libro de trabajo por el id único especificado. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Escribe la cadena JSON del archivo al flujo. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Escribe la cadena JSON del libro de trabajo al flujo |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Escribe la cadena JSON del archivo al flujo por el id único especificado. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Escribe la cadena JSON del libro de trabajo al flujo por el id único especificado. |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Aplica la operación de descarga de archivo |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Obtener flujo de archivo |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | Obtiene la devolución de llamada de advertencia personalizada para la importación de archivo. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Obtener flujo de imagen. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Obtiene la URL de la imagen. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Escribe la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado al flujo.. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Obtiene la cadena JSON del archivo desde la caché usando el ID único especificado, establece el nombre de archivo de salida en el JSON. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Obtiene los datos del arreglo de bytes del objeto OLE incrustado. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | Establece la devolución de llamada de advertencia personalizada para la importación de archivo. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Traduce todos los valores de cadena al idioma objetivo en la hoja de cálculo |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Aplica la operación de actualización. |

### Ver también

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


