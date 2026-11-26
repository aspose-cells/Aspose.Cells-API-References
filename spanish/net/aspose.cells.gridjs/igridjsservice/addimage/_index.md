---
title: "IGridJsService.AddImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IGridJsService. Aplica la operación de agregar imagen desde un archivo local tomando los bytes de la imagen directamente"
type: docs
url: /es/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Aplica la operación de agregar imagen desde archivo local, tomando los bytes de la imagen directamente.

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

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Aplica la operación de agregar imagen desde archivo local, tomando los archivos de formulario cargados.

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

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


