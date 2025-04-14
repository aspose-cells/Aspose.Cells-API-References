﻿---
title: Aspose::Cells::LowCode::AbstractLowCodeLoadOptionsProvider::Finish method
linktitle: Finish
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::LowCode::AbstractLowCodeLoadOptionsProvider::Finish method. Releases resources after processing currently part of input in C++.'
type: docs
weight: 800
url: /cpp/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider::Finish method


Releases resources after processing currently part of input.

```cpp
void Aspose::Cells::LowCode::AbstractLowCodeLoadOptionsProvider::Finish(const LowCodeLoadOptions &part)
```


| Parameter | Type | Description |
| --- | --- | --- |
| part | const LowCodeLoadOptions\& | the load options used for currently split part. |
## Remarks



By default this method just closes the stream specified by the LowCodeLoadOptions.InputStream directly(if the load options
specified a Stream as source). User may overwrite this method to control how to release resources according to their requirement and the implementation of Current. 
## See Also

* Class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* Class [AbstractLowCodeLoadOptionsProvider](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
