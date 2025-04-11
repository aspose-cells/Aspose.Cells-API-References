---
title: AbstractLowCodeSaveOptionsProvider.Finish
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeSaveOptionsProvider method. Releases resources after processing currently split part
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Releases resources after processing currently split part.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Parameter | Type | Description |
| --- | --- | --- |
| part | LowCodeSaveOptions | the save options used for currently split part. |

### Remarks

By default this method just closes the stream specified by the [`OutputStream`](../../lowcodesaveoptions/outputstream/) directly(if the save options specified a Stream as destination). User may overwrite this method to control how to release resources according to their requirement and the implementation of [`GetSaveOptions`](../getsaveoptions/).

### See Also

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


