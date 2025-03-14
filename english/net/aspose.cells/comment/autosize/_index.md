---
title: Comment.AutoSize
second_title: Aspose.Cells for .NET API Reference
description: Comment property. Indicates if size of comment is adjusted automatically according to its content. Note In some special cases such as Mac environment this setting may not take effect. If this setting does not take effect please replace it with FitToTextSize
type: docs
url: /net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### Examples

```csharp

[C#]
if(!comment1.AutoSize)
{
    //The size of the comment varies with the content
    comment1.AutoSize = true;
}
```

### See Also

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


