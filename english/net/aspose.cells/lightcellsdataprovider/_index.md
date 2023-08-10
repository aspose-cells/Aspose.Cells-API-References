---
title: Interface LightCellsDataProvider
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LightCellsDataProvider interface. Represents Data provider for saving large spreadsheet files in light weight mode
type: docs
url: /net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Represents Data provider for saving large spreadsheet files in light weight mode.

```csharp
public interface LightCellsDataProvider
```

## Methods

| Name | Description |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Checks whether the current string value of cell needs to be gathered into a global pool. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Gets next cell to be saved. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Gets the next row to be saved. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Starts to save data of one cell. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Starts to save data of one row. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Starts to save a worksheet. |

### Remarks

When saving a workbook by this mode, [`StartSheet`](./startsheet/) will be checked when saving every worksheet in the workbook. For one sheet, if [`StartSheet`](./startsheet/) gives true, then all data and properties to be saved for rows/cells of this sheet will be provided by the implementation of this interface. In the first place, [`NextRow`](./nextrow/) will be called to get the next row index to be saved. If a valid row index is returned(the row index must be in ascending order for the rows to be saved), then a Row object representing this row will be provided by [`StartRow`](./startrow/) for the implementation to set its properties. For one row, [`NextCell`](./nextcell/) will be checked firstly. If a valid column index be returned(the column index must be in ascending order for all cells of current row), then a Cell object representing this cell will be provided by [`StartCell`](./startcell/) for implementation to set its data and properties. After [`StartCell`](./startcell/) the cell will be saved directly to the resultant spreadsheet file. Then the next cell will be checked and processed.  Please note, user should only update values and properties for current Row/Cell object provided by corresponding method. Because the cells data is written to the resultant file in streaming manner, most of other objects may have been written to the resultant file, or have been gathered and written some global data for them. So when user updating other objects while saving cells data, those operations may be not able to affect the saved data. Or even worse, those operations may cause inconsistent data be save to the resultant file and finally make the file corrupted. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them and adjust them to the final state before calling "Save" method of the Workbook.

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


