---
title: CellsHelper Class 
linktitle: CellsHelper
second_title: Aspose.Cells for Go API Reference
description: 'CellsHelper class. Encapsulates the object that represents cellshelper in Go.'
type: docs
weight: 200
url: /go/aspose.cells/cellshelper/
---

## CellsHelper class

Provides helper functions.

```go

type CellsHelper struct 

cellshelper, _ := asposecells.NewCellsHelper()

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[GetSignificantDigits](./getsignificantdigits/) | Gets and sets the number of significant digits.The default value is 17. | 
|[SetSignificantDigits](./setsignificantdigits/) | Gets and sets the number of significant digits.The default value is 17. | 
|[GetDPI](./getdpi/) | Gets the DPI of the machine. | 
|[SetDPI](./setdpi/) | Gets the DPI of the machine. | 
|[GetTextWidth](./gettextwidth/) | Get width of text in unit of points. | 
|[GetVersion](./getversion/) | Get the release version. | 
|[CellNameToIndex](./cellnametoindex/) | Gets the cell row and column indexes according to its name. | 
|[CellIndexToName](./cellindextoname/) | Gets cell name according to its row and column indexes. | 
|[ColumnIndexToName](./columnindextoname/) | Gets column name according to column index. | 
|[ColumnNameToIndex](./columnnametoindex/) | Gets column index according to column name. | 
|[RowIndexToName](./rowindextoname/) | Gets row name according to row index. | 
|[RowNameToIndex](./rownametoindex/) | Gets row index according to row name. | 
|[GetDateTimeFromDouble](./getdatetimefromdouble/) | Convert the double value to the date time value. | 
|[GetDoubleFromDateTime](./getdoublefromdatetime/) | Convert the date time to double value. | 
|[GetStartupPath](./getstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. | 
|[SetStartupPath](./setstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. | 
|[GetAltStartPath](./getaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. | 
|[SetAltStartPath](./setaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. | 
|[GetLibraryPath](./getlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. | 
|[SetLibraryPath](./setlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. | 
|[CreateSafeSheetName](./createsafesheetname/) | Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with ' ', then return the rebuilt string value. | 
|[CreateSafeSheetName](./createsafesheetname/) | Checks given sheet name and create a valid one when needed.If given sheet name conforms to the rules of excel sheet name, then return it.Otherwise string will be truncated if length exceeds the limitand invalid characters will be replaced with given character, then return the rebuilt string value. | 
|[NeedQuoteInFormula](./needquoteinformula/) | Indicates whether the name of the sheet should be enclosed in single quotes | 
|[IsCloudPlatform](./iscloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, | 
|[SetIsCloudPlatform](./setiscloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, | 
