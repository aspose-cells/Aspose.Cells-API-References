---
title: StartCell
second_title: Справочник по Aspose.Cells для .NET API
description: Готовится к обработке ячейки.
type: docs
weight: 30
url: /ru/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Готовится к обработке ячейки.

```csharp
public bool StartCell(int columnIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | Int32 | индекс столбца ячейки для обработки |

### Возвращаемое значение

нужно ли обрабатывать эту ячейку. false, чтобы игнорировать ячейку и проверять следующую, пока не будут достигнуты данные ячеек текущей строки

### Примечания

Будет вызываться при достижении существующей ячейки в текущей строке. Текущая строка — это строка последнего вызова[`ProcessRow`](../processrow) .

### Смотрите также

* interface [LightCellsDataHandler](../../lightcellsdatahandler)
* пространство имен [Aspose.Cells](../../lightcellsdatahandler)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
