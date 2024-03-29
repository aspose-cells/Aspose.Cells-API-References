---
title: LightCellsDataProvider.StartRow
second_title: Aspose.Cells for .NET API Reference
description: LightCellsDataProvider method. Starts to save data of one row
type: docs
url: /net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Starts to save data of one row.

```csharp
public void StartRow(Row row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Row | Row object for implementation to fill data. Its row index is the returned value of latest call of [`NextRow`](../nextrow/). If the row has been initialized in the inner cells model, the existing row object will be used. Otherwise a temporary Row object will be used for implementation to fill data. |

### Remarks

It will be called at the beginning of saving a row and its cells data. If current row has some custom properties such as height, style, ...etc., implementation should set those properties to given Row object here.

### See Also

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


