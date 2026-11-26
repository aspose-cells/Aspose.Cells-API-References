---
title: "MainWeb.SessionMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MainWeb. Obtiene o establece el modo de sesión de la cuadrícula"
type: docs
url: /es/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

Obtiene o establece el modo de sesión de la cuadrícula.

```csharp
public SessionMode SessionMode { get; set; }
```

### Observaciones

Hay 4 tipos de modo de sesión: 1. Session(default): Usa la sesión del sistema para almacenar los datos de la hoja. Generalmente asp.net usa el estado de sesión InProc. La cuadrícula también soporta el estado de sesión "StateServer" fuera del proceso y el estado de sesión SQLServer. 2. ViewState: Usa el viewstate de la página para almacenar los datos de la hoja. 3. Custom: Usa los eventos LoadCustomData y SheetDataUpdated para almacenar/recuperar los datos de la hoja. 4. File: almacena/recupera los datos de la hoja en SessionStorePath. Esta es la forma recomendada y puede mantener el archivo siempre. Al usar SessionMode.ViewState, la cuadrícula almacenará algunos datos en el viewstate de la página. Esto reducirá el uso de memoria del servidor, pero el tamaño de la página será mayor y afectará el rendimiento general.

### Ejemplos

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### Ver también

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


