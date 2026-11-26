---
title: "MainWeb.OnSubmitClientFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MainWeb propiedad. Obtiene o establece la función del cliente que se llamará antes de que el control se envíe del lado del cliente. La función del cliente debe declararse así: function MyOnSubmitarg cancelEdit  return true El argumento arg es el argumento de envío que contiene el comando a publicar en el servidor. cancelEdit es un valor booleano que indica si el control ha descartado la entrada del usuario antes del envío. El control continuará enviando si la función devuelve true. Nota: Puede usar el puntero this en la función del cliente para referirse al control de cuadrícula que dispara el evento"
type: docs
url: /es/net/aspose.cells.gridweb/mainweb/onsubmitclientfunction/
---
## MainWeb.OnSubmitClientFunction property

Obtiene o establece la función del cliente que se llamará antes de que el control se envíe del lado del cliente. La función del cliente debe declararse así: function MyOnSubmit(arg, cancelEdit) { return true;} El parámetro arg es el argumento de envío, contiene el comando que se enviará al servidor. cancelEdit es un valor booleano que indica si el control ha descartado la entrada del usuario antes del envío. El control continuará enviando si la función devuelve true. Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

```csharp
public string OnSubmitClientFunction { get; set; }
```

### Ver también

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


