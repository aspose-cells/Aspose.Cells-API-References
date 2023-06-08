---
title: TextBoxCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: TextBoxCollection property. Gets the TextBox element at the specified index
type: docs
url: /net/aspose.cells.drawing/textboxcollection/item/
---
## TextBoxCollection indexer (1 of 2)

Gets the [`TextBox`](../../textbox/) element at the specified index.

```csharp
public TextBox this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp

[C#]
int index = textBoxCollection.Count - 1;
TextBox txb = textBoxCollection[index];
```

### See Also

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## TextBoxCollection indexer (2 of 2)

Gets the [`TextBox`](../../textbox/) element by the name.

```csharp
public TextBox this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the text box. |

### Examples

```csharp

[C#]
string txtboxName = "textbox 1"; 
TextBox txb2 = textBoxCollection[txtboxName];
if(txb2 != null)
{
    //do what you want
}
```

### See Also

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


