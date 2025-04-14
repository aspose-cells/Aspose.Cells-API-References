﻿---
title: Aspose::Cells::LowCode::AbstractLowCodeSaveOptionsProvider::Finish method
linktitle: Finish
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::LowCode::AbstractLowCodeSaveOptionsProvider::Finish method. Releases resources after processing currently split part in C++.'
type: docs
weight: 700
url: /cpp/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider::Finish method


Releases resources after processing currently split part.

```cpp
void Aspose::Cells::LowCode::AbstractLowCodeSaveOptionsProvider::Finish(const LowCodeSaveOptions &part)
```


| Parameter | Type | Description |
| --- | --- | --- |
| part | const LowCodeSaveOptions\& | the save options used for currently split part. |
## Remarks



By default this method just closes the stream specified by the LowCodeSaveOptions.OutputStream directly(if the save options
specified a Stream as destination). User may overwrite this method to control how to release resources according to their requirement and the implementation of GetSaveOptions(SplitPartInfo). 
## See Also

* Class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* Class [AbstractLowCodeSaveOptionsProvider](../)
* Namespace [Aspose::Cells::LowCode](../../)
* Library [Aspose.Cells for C++](../../../)
