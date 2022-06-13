---
title: IsGatherString
second_title: Справочник по Aspose.Cells для .NET API
description: Проверяет нужно ли собирать текущее строковое значение ячейки в глобальный пул.
type: docs
weight: 10
url: /ru/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Проверяет, нужно ли собирать текущее строковое значение ячейки в глобальный пул.

```csharp
public bool IsGatherString()
```

### Возвращаемое значение

true, если строковое значение необходимо собрать в глобальный пул для результирующего файла.

### Примечания

Сбор строковых значений будет иметь преимущество только тогда, когда имеется много повторяющихся строковых значений для ячеек, предоставленных этим реализация. В этой ситуации сбор строки сэкономит много памяти и создаст результирующий файл меньшего размера. Если имеется много строковых значений для ячеек, предоставляемых LightCellsDataProvider, но лишь немногие из них одинаковы, сбор строки будет стоить больше памяти и времени и не будет иметь преимущества для результирующего файла.

### Смотрите также

* interface [LightCellsDataProvider](../../lightcellsdataprovider)
* пространство имен [Aspose.Cells](../../lightcellsdataprovider)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->