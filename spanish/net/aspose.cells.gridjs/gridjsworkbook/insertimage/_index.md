---
title: "GridJsWorkbook.InsertImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de GridJsWorkbook. Inserta una imagen en la hoja de cálculo desde el flujo de archivo o la URL; se debe proporcionar el flujo de archivo o la URL, o inserta una forma cuando p.type es uno de AutoShapeType"
type: docs
url: /es/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

Inserta una imagen en la hoja de cálculo desde un flujo de archivo o la URL (se debe proporcionar el flujo de archivo o la URL), o inserta una forma cuando p.type es uno de AutoShapeType

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | String | El id único para la caché de archivos |
| p | String | La cadena con formato JSON para la operación que especifica la ubicación de la celda, el nombre de la hoja de cálculo, fila superior izquierda, columna superior izquierda para la imagen, etc {name:'sheet1',ri:1,ci:1} |
| s | Stream | El flujo de archivo del archivo de imagen |
| imageUrl | String | La URL del archivo de imagen |

### Valor de retorno

La cadena con formato JSON de la imagen insertada

### Ver también

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


