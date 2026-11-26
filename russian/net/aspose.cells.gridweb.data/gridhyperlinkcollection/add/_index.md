---
title: "GridHyperlinkCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridHyperlinkCollection. Добавляет гиперссылку в указанную ячейку или диапазон ячеек"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Первая строка диапазона гиперссылки. |
| firstColumn | Int32 | Первый столбец диапазона гиперссылки. |
| totalRows | Int32 | Количество строк в этом диапазоне гиперссылки. |
| totalColumns | Int32 | Количество столбцов этого диапазона гиперссылки. |
| address | String | Адрес гиперссылки. |

### Возвращаемое значение

[`GridHyperlink`](../../gridhyperlink/) object index.

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, int, int, string) {#add_1}

Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |
| totalRows | Int32 | Количество строк в этом диапазоне гиперссылки. |
| totalColumns | Int32 | Количество столбцов этого диапазона гиперссылки. |
| address | String | Адрес гиперссылки. |

### Возвращаемое значение

[`GridHyperlink`](../../gridhyperlink/) object index.

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string) {#add_2}

Добавляет гиперссылку в указанную ячейку.

```csharp
public int Add(string cellName, string address)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |
| address | String | Адрес гиперссылки. |

### Возвращаемое значение

[`GridHyperlink`](../../gridhyperlink/) object index.

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startCellName | String | Ячейка в левом верхнем углу диапазона. |
| endCellName | String | Ячейка в правом нижнем углу диапазона. |
| address | String | Адрес гиперссылки. |
| textToDisplay | String | Текст, который будет отображаться для указанной гиперссылки. |
| screenTip | String | Текст screenTip для указанной гиперссылки. |

### Возвращаемое значение

[`GridHyperlink`](../../gridhyperlink/) object index.

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


