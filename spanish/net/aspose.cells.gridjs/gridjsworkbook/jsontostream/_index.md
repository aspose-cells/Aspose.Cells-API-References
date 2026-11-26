---
title: "GridJsWorkbook.JsonToStream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridJsWorkbook. Genera JSON a partir del Libro de trabajo en memoria y lo escribe en el flujo especificado. Opcionalmente almacena en caché el JSON generado para una recuperación posterior más rápida. Diferencias clave con JsonToStreamByUid: este método usa el estado actual del Libro de trabajo en memoria (campo wb). JsonToStreamByUid recarga el Libro de trabajo desde los archivos de caché .cells en disco. Use este método cuando desee exportar el estado actual del libro de trabajo después de modificaciones. Use JsonToStreamByUid cuando necesite regenerar JSON a partir de un estado de archivo previamente almacenado en caché. Comportamiento de caché cuando se proporciona uid: verifica la caché JSON antes de generar (L1 memoria, L2 disco). Si hay una falta de caché, genera JSON desde el libro de trabajo en memoria. Almacena el JSON generado en caché para futuras solicitudes."
type: docs
url: /es/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

Genera JSON a partir del Workbook en memoria y lo escribe en el flujo especificado. Opcionalmente almacena en caché el JSON generado para una recuperación posterior más rápida. Diferencias clave con JsonToStreamByUid: - Este método usa el estado actual del Workbook en memoria (campo wb) - JsonToStreamByUid recarga el Workbook desde los archivos de caché .cells en disco - Usa este método cuando deseas exportar el estado actual del libro después de modificaciones - Usa JsonToStreamByUid cuando necesitas regenerar JSON a partir de un estado de archivo previamente almacenado en caché. Comportamiento de caché (cuando se proporciona uid): - Verifica la caché de JSON antes de generar (memoria L1 + disco L2) - Si hay una falta de caché, genera JSON desde el workbook en memoria - Almacena el JSON generado en la caché para futuras solicitudes

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de salida donde escribir los datos JSON. |
| nombre de archivo | String | Especifica el nombre de archivo en el JSON. Si se establece a null, el nombre de archivo predeterminado es: book1. |
| uid | String | Identificador único opcional para el caché JSON. Cuando se proporciona, habilita la búsqueda y el almacenamiento en caché. |

### Ver también

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


