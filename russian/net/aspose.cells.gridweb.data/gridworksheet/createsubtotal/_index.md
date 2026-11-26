---
title: "GridWorksheet.CreateSubtotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridWorksheet. Создает промежуточный итог на листе"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## CreateSubtotal(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) {#createsubtotal_1}

Создаёт промежуточный итог на листе.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Индекс строки, содержащей название столбца. |
| dataRows | Int32 | Количество строк данных. |
| groupByColumnIndex | Int32 | Индекс столбца, который будет группироваться. |
| subtotalFunction | SubtotalFunction | Тип функции подытога. |
| subtotalColumnIndexList | Int32[] | Индексы столбцов, подлежащих подытогу. |
| functionLabel | String | Метка функции подытога. |
| grandCellStyle | GridTableItemStyle | Стиль строки общего итога. |
| subtotalCellStyle | GridTableItemStyle | Стиль строки подытога. |
| numberType | NumberType | Тип числа ячеек результата подытога. |
| customString | String | Строка пользовательского формата ячеек результата подытога. Может быть null. |

### См. также

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreateSubtotal(int, int, int, SubtotalFunction, int[]) {#createsubtotal}

Создаёт промежуточный итог на листе.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Индекс строки, содержащей название столбца. |
| dataRows | Int32 | Количество строк данных. |
| groupByColumnIndex | Int32 | Индекс столбца, который будет группироваться. |
| subtotalFunction | SubtotalFunction | Тип функции подытога. |
| subtotalColumnIndexList | Int32[] | Индексы столбцов, подлежащих подытогу. |

### См. также

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


