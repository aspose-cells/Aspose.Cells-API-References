---
title: LightCellsDataProvider.IsGatherString
second_title: Aspose.Cells for .NET API Reference
description: LightCellsDataProvider method. Checks whether the current string value of cell needs to be gathered into a global pool
type: docs
url: /net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Checks whether the current string value of cell needs to be gathered into a global pool.

```csharp
public bool IsGatherString()
```

### Return Value

true if string value need to be gathered into a global pool for the resultant file.

### Remarks

Gathering string values will take advantage only when there are many duplicated string values for the cells provided by this implementation. In this situation gathering string will save much memory and generate smaller resultant file. If there are many string values for the cells provided by LightCellsDataProvider but few of them are same, gathering string will cost more memory and time and has no advantage for the resultant file.

### See Also

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


