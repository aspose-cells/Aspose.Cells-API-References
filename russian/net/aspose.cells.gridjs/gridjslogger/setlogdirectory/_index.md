---
title: "GridJsLogger.SetLogDirectory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridJsLogger. Устанавливает каталог журнала с ежедневной стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться gridjs_period.log"
type: docs
url: /ru/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Устанавливает каталог журналов с ежедневной стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | String | Каталог для хранения файлов журнала. |

### См. также

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Устанавливает каталог журналов со стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | String | Каталог для хранения файлов журнала. |
| rolling | GridJsLogRolling | Стратегия ротации (Daily/Weekly/Monthly). |

### См. также

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Устанавливает каталог журналов со стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться: {prefix}_{period}.log Примеры: gridjs_2026-07-27.log (ежедневно), gridjs_2026-W30.log (еженедельно), gridjs_2026-07.log (ежемесячно).

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | String | Каталог для хранения файлов журнала. |
| rolling | GridJsLogRolling | Стратегия ротации (Daily/Weekly/Monthly). |
| filePrefix | String | Префикс имени файла. |

### См. также

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


