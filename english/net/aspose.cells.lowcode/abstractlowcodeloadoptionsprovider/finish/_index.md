---
title: AbstractLowCodeLoadOptionsProvider.Finish
second_title: Aspose.Cells for .NET API Reference
description: AbstractLowCodeLoadOptionsProvider method. Releases resources after processing currently part of input
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Releases resources after processing currently part of input.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Parameter | Type | Description |
| --- | --- | --- |
| part | LowCodeLoadOptions | the load options used for currently split part. |

### Remarks

By default this method just closes the stream specified by the [`InputStream`](../../lowcodeloadoptions/inputstream/) directly(if the load options specified a Stream as source). User may overwrite this method to control how to release resources according to their requirement and the implementation of [`Current`](../current/).

### See Also

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


