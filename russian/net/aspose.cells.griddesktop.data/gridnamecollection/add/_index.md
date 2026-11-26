---
title: "GridNameCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "GridNameCollection метод. Определяет новое глобальное имя"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

Определяет новое глобальное имя.

```csharp
public int Add(string text, string refersTo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | Name текст. Может иметь имя листа . |
| refersTo | String | Формула, к которой определено имя. Должна иметь имя листа, например, 'sheet hello!'A1:B2. |

### Возвращаемое значение

Индекс объекта Name.

### См. также

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, string, string) {#add}

Определяет новое имя в указанном листе.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Параметр | Описание |
| --- | --- |
| sheetIndex | Индекс листа, в котором применяется имя. |
| текст | Name текст. Не может иметь имя листа . |
| refersTo | Формула, к которой определено имя. Должна иметь имя листа, например, 'sheet hello!'A1:B2. |
| sheetIndex | Name's SheetIndex ,индекс начинается с 1. |

### Возвращаемое значение

Индекс объекта Name.

### См. также

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


