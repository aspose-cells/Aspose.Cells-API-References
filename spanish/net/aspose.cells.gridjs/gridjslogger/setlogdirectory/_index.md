---
title: "GridJsLogger.SetLogDirectory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridJsLogger. Establece el directorio de registro con estrategia de archivo rotativo diario y habilita la salida a archivo. Los archivos de registro se nombrarán como gridjs_period.log"
type: docs
url: /es/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Establece el directorio de registro con estrategia de rotación diaria y habilita la salida a archivo. Los archivos de registro se nombrarán como: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | String | El directorio donde se almacenarán los archivos de registro. |

### Ver también

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Establece el directorio de registro con estrategia de rotación y habilita la salida a archivo. Los archivos de registro se nombrarán como: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | String | El directorio donde se almacenarán los archivos de registro. |
| rotación | GridJsLogRolling | La estrategia de rotación (Diario/Semanal/Mensual). |

### Ver también

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Establece el directorio de registro con estrategia de rotación y habilita la salida a archivo. Los archivos de registro se nombrarán como: {prefix}_{period}.log Ejemplos: gridjs_2026-07-27.log (Diario), gridjs_2026-W30.log (Semanal), gridjs_2026-07.log (Mensual)

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | String | El directorio donde se almacenarán los archivos de registro. |
| rotación | GridJsLogRolling | La estrategia de rotación (Diario/Semanal/Mensual). |
| filePrefix | String | El prefijo del nombre de archivo. |

### Ver también

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


