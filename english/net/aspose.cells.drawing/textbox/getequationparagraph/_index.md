---
title: TextBox.GetEquationParagraph
second_title: Aspose.Cells for .NET API Reference
description: TextBox method. Get the specified math paragraph from the TextBody property of the TextBox object. Notice 1 Returns NULL when the index is out of bounds or not found. 2 Also returns NULL if the specified index position is not a math paragraph
type: docs
url: /net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

Get the specified math paragraph from the TextBody property of the TextBox object. Notice: (1) Returns NULL when the index is out of bounds or not found. (2) Also returns NULL if the specified index position is not a math paragraph.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The position index of the math paragraph, starting from 0. |

### Return Value

Returns the math paragraph specified by index.

### See Also

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

Gets the first math paragraph from the TextBody property of the TextBox object.

```csharp
public EquationNode GetEquationParagraph()
```

### Return Value

If there has math paragraph, returns the first one, otherwise returns null.

### See Also

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


