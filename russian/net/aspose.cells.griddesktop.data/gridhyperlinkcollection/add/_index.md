---
title: "GridHyperlinkCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridHyperlinkCollection. Добавляет гиперссылку в указанную ячейку или диапазон ячеек"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
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

Индекс объекта гиперссылки.

### Примеры

```csharp
[C#]

Worksheet worksheet = excel.Worksheets[0];
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls");

[Visual Basic]

Dim worksheet as Worksheet = excel.Worksheets(0)
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com")
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls")

```

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Индекс объекта гиперссылки.

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Индекс объекта гиперссылки.

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Индекс объекта гиперссылки.

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

Добавляет гиперссылку в указанную ячейку по индексу строки и столбца.

```csharp
public void Add(int row, int col, string url)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки ячейки. |
| col | Int32 | Индекс столбца ячейки. |
| url | String | URL гиперссылки. |

### См. также

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


