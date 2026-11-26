---
title: "GridNameCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "GridNameCollection метод. Определяет новое глобальное имя"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridnamecollection/add/
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
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(int, string, string) {#add}

Определяет новое имя в указанном листе.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс листа, в котором применяется имя. |
| текст | String | Name текст. Не может иметь имя листа . |
| refersTo | String | Формула, к которой определено имя. Должна иметь имя листа, например, 'sheet hello!'A1:B2. |

### Возвращаемое значение

Индекс объекта Name.

### См. также

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


