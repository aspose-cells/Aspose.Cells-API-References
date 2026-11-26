---
title: "Worksheet.AddCustomFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Добавляет пользовательский фильтр для указанного диапазона строк от начальной строки до конечной строки"
type: docs
url: /ru/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Добавляет пользовательский фильтр для указанного диапазона строк от начальной строки до конечной.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startrow | Int32 | Начальная строка диапазона фильтра |
| startcolumn | Int32 | Начальный столбец диапазона фильтра |
| critiras | Object[] | Массив critira для столбцов, каждый применяется к каждому столбцу |
| filterOperatorTypes | GridFilterOperatorType[] | Массив типов операций фильтра для столбцов, каждый применяется к каждому столбцу |

### См. также

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Добавить пользовательский фильтр для указанной строки.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Примечания

Строка критериев фильтра. Обратите внимание, что мы используем запятую и точку с запятой в качестве разделителей, поэтому значение ячейки не должно содержать эти символы. Ниже приведены примеры строк критериев: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


