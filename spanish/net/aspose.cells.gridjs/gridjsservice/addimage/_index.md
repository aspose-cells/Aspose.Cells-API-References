---
title: "GridJsService.AddImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de GridJsService. Aplica la adición de imagen desde un archivo local; los bytes del archivo provienen de JS FormData o cualquier host"
type: docs
url: /es/net/aspose.cells.gridjs/gridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Aplica la operación de agregar imagen desde archivo local (los bytes del archivo provienen de JS FormData o cualquier host).

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | String | El parámetro de cadena JSON |
| uid | String | El identificador único para la caché del archivo. |
| iscontrol | String | Especifique si es un control. |
| fileBytes | Byte[] | Los bytes sin procesar del archivo de imagen |

### Valor de retorno

El resultado de cadena JSON

### Ver también

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Aplica la operación de agregar imagen desde archivo local.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | String | El parámetro de cadena JSON |
| uid | String | El identificador único para la caché del archivo. |
| iscontrol | String | Especifique si es un control. |
| archivos | IFormFileCollection | El archivo de formulario de la imagen |

### Valor de retorno

El resultado de cadena JSON

### Ver también

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


