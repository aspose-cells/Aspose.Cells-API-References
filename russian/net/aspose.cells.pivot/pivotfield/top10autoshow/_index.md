---
title: "PivotField.Top10AutoShow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Настраивает параметры Top10 AutoShow для этого поля сводки"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Настраивает параметры Top10 AutoShow для этого сводного поля.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isAutoShow | Boolean | true — включить AutoShow; false — отключить. |
| isTop | Boolean | Если true, показываются верхние элементы; false — нижние элементы. |
| количество | Int32 | Количество отображаемых верхних/нижних элементов. |
| rankBy | Int32 | Индекс поля данных, используемого для ранжирования. Используйте -1 для ранжирования по собственным значениям pivotItem. |

### Примечания

Этот метод настраивает [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

Бинарный формат XLS: AutoShow (Top10) является нативным и единственным поддерживаемым вариантом.

XLSX (OpenXML): Основной формат файла поддерживает Top10 AutoShow, но пользовательский интерфейс Excel 2007 и новее отображает это только через фильтр Top10. Если совместимость с XLS не требуется, рекомендуется использовать фильтр Top10.

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


