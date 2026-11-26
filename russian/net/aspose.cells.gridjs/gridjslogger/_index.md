---
title: "Класс GridJsLogger"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridJs.GridJsLogger. Предоставляет лёгкую систему логирования для сервера GridJs. Поддерживает вывод в консоль и в файл с настраиваемыми уровнями журналирования. Уровень по умолчанию — None. В сборке DEBUG уровень по умолчанию — Debug, выводит все сообщения. Поддерживает ротацию файлов журнала по дню/неделе/месяцу."
type: docs
url: /ru/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

Предоставляет облегченную систему логирования для сервера GridJs. Поддерживает вывод в консоль и файл с настраиваемыми уровнями логирования. Уровень по умолчанию — None. В сборке DEBUG уровень по умолчанию — Debug (выводит все сообщения). Поддерживает ротацию файлов журнала по дню/неделе/месяцу.

```csharp
public static class GridJsLogger
```

## Свойства

| Имя | Описание |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Получает или устанавливает, выводить ли сообщения журнала в консоль. По умолчанию — false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Получает или устанавливает, выводить ли сообщения журнала в файл. По умолчанию — false. Необходимо вызвать [`SetLogFile`](./setlogfile/) или [`SetLogDirectory`](./setlogdirectory/) перед включением. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Получает или устанавливает минимальный уровень журнала. Сообщения ниже этого уровня будут игнорироваться. По умолчанию — None. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Получает текущий путь к файлу журнала или null, если не установлен. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Получает или устанавливает максимальный размер (в байтах) одного файла журнала перед ротацией. Действует только когда ротация включена. 0 означает отсутствие ограничения размера. По умолчанию — 0. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Закрывает запись в файл журнала и отключает вывод в файл. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Записывает сообщение уровня debug. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Записывает сообщение уровня error. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Записывает сообщение уровня info. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Записывает сообщение на указанном уровне. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Устанавливает каталог журналов с ежедневной стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Устанавливает каталог журналов со стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Устанавливает каталог журналов со стратегией ротации файлов и включает вывод в файл. Файлы журнала будут называться: {prefix}_{period}.log Примеры: gridjs_2026-07-27.log (ежедневно), gridjs_2026-W30.log (еженедельно), gridjs_2026-07.log (ежемесячно). |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Устанавливает путь к файлу журнала и включает вывод в файл (режим единственного файла, без ротации). Добавляет записи к существующему файлу. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Устанавливает путь к файлу журнала и включает вывод в файл (режим единственного файла, без ротации). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Записывает сообщение уровня предупреждения. |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


