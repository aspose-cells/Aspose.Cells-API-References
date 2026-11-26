---
title: "Enumeración SessionMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.SessionMode enum. Representa el modo de sesión de la cuadrícula"
type: docs
url: /es/net/aspose.cells.gridweb/sessionmode/
---
## SessionMode enumeration

Representa el modo de sesión de la cuadrícula.

```csharp
public enum SessionMode
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Session | `0` | Utiliza la sesión del sistema para almacenar/recuperar los datos de la hoja de la cuadrícula automáticamente. |
| ViewState | `1` | Utiliza el viewstate de la página para almacenar/recuperar los datos de la hoja de la cuadrícula automáticamente. |
| Custom | `2` | Utiliza el evento LoadCustomData para cargar manualmente los datos de la hoja de la cuadrícula. Y utiliza el evento SheetDataUpdated para guardar los datos de la hoja de la cuadrícula. |
| File | `3` | Utiliza el archivo del sistema para almacenar/recuperar los datos de la hoja de la cuadrícula automáticamente, el usuario necesita establecer SessionStorePath para especificar el directorio del archivo. |

### Ver también

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


