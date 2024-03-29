---
title: Add
second_title: Справочник по Aspose.Cells для .NET API
description: Добавляет комментарий в коллекцию.
type: docs
weight: 20
url: /ru/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Добавляет комментарий в коллекцию.

```csharp
public int Add(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| row | Int32 | Индекс строки ячейки. |
| column | Int32 | Индекс столбца ячейки. |

### Возвращаемое значение

[`Comment`](../../comment) индекс объекта.

### Примеры

```csharp

[C#]
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";
```

### Смотрите также

* class [CommentCollection](../../commentcollection)
* пространство имен [Aspose.Cells](../../commentcollection)
* сборка [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Добавляет комментарий в коллекцию.

```csharp
public int Add(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Возвращаемое значение

[`Comment`](../../comment) индекс объекта.

### Примеры

```csharp

[C#]
int commentIndex2 = comments.Add("B2");
Comment comment2 = comments[commentIndex2];
comment2.Note = "Second note.";
comment2.Font.Name = "Times New Roman";
```

### Смотрите также

* class [CommentCollection](../../commentcollection)
* пространство имен [Aspose.Cells](../../commentcollection)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
