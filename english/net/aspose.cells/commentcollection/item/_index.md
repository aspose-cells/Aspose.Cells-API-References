---
title: CommentCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: CommentCollection property. Gets the Comment element at the specified index
type: docs
url: /net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Gets the [`Comment`](../../comment/) element at the specified index.

```csharp
public Comment this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp

[C#]
Comment comment3 = comments[0];
comment3.Note = "Three note.";
```

### See Also

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Gets the [`Comment`](../../comment/) element at the specified cell.

```csharp
public Comment this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | Cell name. |

### Return Value

The element at the specified cell.

### Examples

```csharp

[C#]
Comment comment4 = comments["B2"];
comment4.Note = "Four note.";
```

### See Also

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Gets the [`Comment`](../../comment/) element at the specified row index and column index.

```csharp
public Comment this[int row, int column] { get; }
```

| Parameter | Description |
| --- | --- |
| row | Row index. |
| column | Column index. |

### Return Value

The element at the specified cell.

### Examples

```csharp

[C#]
Comment comment5 = comments[1,1];
comment5.Note = "Five note.";
```

### See Also

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


