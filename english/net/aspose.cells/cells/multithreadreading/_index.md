---
title: Cells.MultiThreadReading
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets whether the cells data model should support MultiThread reading. Default value of this property is false
type: docs
url: /net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Remarks

If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


