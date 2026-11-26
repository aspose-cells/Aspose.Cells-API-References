---
title: "Interfaz IGridJsService"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridJs.IGridJsService interfaz. Representa la interfaz básica de APIs de operación utilizada en acciones de controlador."
type: docs
url: /es/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

Representa la interfaz de API básicas de operación utilizadas en acciones de controlador.

```csharp
public interface IGridJsService : IDisposable
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | Aplica la operación de agregar imagen desde archivo local, tomando los bytes de la imagen directamente. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Aplica la operación de agregar imagen desde archivo local, tomando los archivos de formulario cargados. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | Aplica la operación de agregar imagen desde URL remota. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Comprueba si la instancia del libro de trabajo está en la caché de memoria. este método se aplica solo para el modo colaborativo. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | Elimina todas las entradas de caché JSON (memoria y disco). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | Elimina todas las entradas de caché JSON que pertenecen al id único especificado. Llame a esto después de modificar el archivo fuente fuera de banda para que la siguiente solicitud regenere el JSON. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Aplica la operación de copiar imagen. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Obtiene la cadena JSON del archivo por el id único especificado. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Obtiene la cadena JSON del libro de trabajo por el id único especificado. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Escribe la cadena JSON del libro de trabajo al flujo |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Escribe la cadena JSON del libro de trabajo al flujo |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Escribe la cadena JSON del archivo al flujo por el id único especificado. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Escribe la cadena JSON del libro de trabajo al flujo por el id único especificado. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Aplica la operación de descarga de archivo |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Obtener flujo de archivo |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | Obtiene la devolución de llamada de advertencia personalizada para la importación de archivo. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Obtener flujo de imagen. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Obtiene la URL de la imagen. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Obtiene la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Escribe la cadena JSON de la hoja especificada en el archivo desde la caché usando el ID único especificado al flujo.. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Obtiene la cadena JSON del archivo desde la caché usando el ID único especificado, establece el nombre de archivo de salida en el JSON. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Obtiene los datos del arreglo de bytes del objeto OLE incrustado. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | Establece la devolución de llamada de advertencia personalizada para la importación de archivo. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Aplica la operación de actualización. |

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


