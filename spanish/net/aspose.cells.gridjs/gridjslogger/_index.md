---
title: "Clase GridJsLogger"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridJs.GridJsLogger. Proporciona un sistema de registro ligero para el servidor GridJs. Soporta salida a consola y a archivo con niveles de registro configurables. El nivel predeterminado es None. En una compilación DEBUG, el nivel predeterminado es Debug y muestra todos los mensajes. Soporta la rotación de archivos de registro por día/semana/mes."
type: docs
url: /es/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

Proporciona un sistema de registro ligero para el servidor GridJs. Soporta salida a consola y archivo con niveles de registro configurables. El nivel predeterminado es None. En compilación DEBUG, el nivel predeterminado es Debug (muestra todos los mensajes). Soporta la rotación de archivos de registro por día/semana/mes.

```csharp
public static class GridJsLogger
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Obtiene o establece si se deben enviar los mensajes de registro a la consola. El valor predeterminado es false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Obtiene o establece si se deben enviar los mensajes de registro a un archivo. El valor predeterminado es false. Debe llamarse a [`SetLogFile`](./setlogfile/) o a [`SetLogDirectory`](./setlogdirectory/) antes de habilitarlo. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Obtiene o establece el nivel mínimo de registro. Los mensajes por debajo de este nivel se ignorarán. El valor predeterminado es None. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Obtiene la ruta actual del archivo de registro, o null si no está configurada. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Obtiene o establece el tamaño máximo (en bytes) para un solo archivo de registro antes de rotar. Solo es efectivo cuando la rotación está habilitada. 0 significa sin límite de tamaño. El valor predeterminado es 0. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Cierra el escritor del archivo de registro y deshabilita la salida a archivo. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Registra un mensaje a nivel de depuración. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Registra un mensaje a nivel de error. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Registra un mensaje a nivel informativo. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Registra un mensaje en el nivel especificado. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Establece el directorio de registro con estrategia de rotación diaria y habilita la salida a archivo. Los archivos de registro se nombrarán como: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Establece el directorio de registro con estrategia de rotación y habilita la salida a archivo. Los archivos de registro se nombrarán como: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Establece el directorio de registro con estrategia de rotación y habilita la salida a archivo. Los archivos de registro se nombrarán como: {prefix}_{period}.log Ejemplos: gridjs_2026-07-27.log (Diario), gridjs_2026-W30.log (Semanal), gridjs_2026-07.log (Mensual) |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Establece la ruta del archivo de registro y habilita la salida a archivo (modo de archivo único, sin rotación). Añade al archivo existente. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Establece la ruta del archivo de registro y habilita la salida a archivo (modo de archivo único, sin rotación). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Registra un mensaje de nivel de advertencia. |

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


