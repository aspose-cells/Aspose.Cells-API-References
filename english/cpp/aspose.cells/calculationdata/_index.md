---
title: Aspose::Cells::CalculationData class
linktitle: CalculationData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CalculationData class. Represents the required data when calculating one function, such as function name, parameters, ...etc in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells/calculationdata/
---
## CalculationData class


Represents the required data when calculating one function, such as function name, parameters, ...etc.

```cpp
class CalculationData
```

## Methods

| Method | Description |
| --- | --- |
| [CalculationData(CalculationData_Impl* impl)](./calculationdata/) | Constructs from an implementation object. |
| [CalculationData(const CalculationData\& src)](./calculationdata/) | Copy constructor. |
| [GetCalculatedValue()](./getcalculatedvalue/) | Gets or sets the calculated value for this function. |
| [GetCell()](./getcell/) | Gets the [Cell](../cell/) object where the function is. |
| [GetCellColumn()](./getcellcolumn/) | Gets the column index of the cell where the function is. |
| [GetCellRow()](./getcellrow/) | Gets the row index of the cell where the function is. |
| [GetFunctionName()](./getfunctionname/) | Gets the function name to be calculated. |
| [GetParamCount()](./getparamcount/) | Gets the count of parameters. |
| [GetParamText(int32_t index)](./getparamtext/) | Gets the literal text of the parameter at the given index. |
| [GetParamValue(int32_t index)](./getparamvalue/) | Gets the represented value object of the parameter at a given index. |
| [GetParamValueInArrayMode(int32_t index, int32_t maxRowCount, int32_t maxColumnCount)](./getparamvalueinarraymode/) | Gets the value(s) of the parameter at a given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode. |
| [GetWorkbook()](./getworkbook/) | Gets the [Workbook](../workbook/) object where the function is. |
| [GetWorksheet()](./getworksheet/) | Gets the [Worksheet](../worksheet/) object where the function is. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CalculationData\& src)](./operator_asm/) | operator= |
| [SetCalculatedValue(const Aspose::Cells::Object\& value)](./setcalculatedvalue/) | Gets or sets the calculated value for this function. |
| [~CalculationData()](./~calculationdata/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks


All objects provided by this class are for "read" purpose only. User should not change any data in the [Workbook](../workbook/) during the formula calculation process, Otherwise unexpected result or Exception may be caused.
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
