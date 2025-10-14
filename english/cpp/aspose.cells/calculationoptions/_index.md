---
title: Aspose::Cells::CalculationOptions class
linktitle: CalculationOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CalculationOptions class. Represents options for calculation in C++.'
type: docs
weight: 1300
url: /cpp/aspose.cells/calculationoptions/
---
## CalculationOptions class


Represents options for calculation.

```cpp
class CalculationOptions
```

## Methods

| Method | Description |
| --- | --- |
| [CalculationOptions()](./calculationoptions/) | Default constructor. |
| [CalculationOptions(CalculationOptions_Impl* impl)](./calculationoptions/) | Constructs from an implementation object. |
| [CalculationOptions(const CalculationOptions\& src)](./calculationoptions/) | Copy constructor. |
| [GetCalcStackSize()](./getcalcstacksize/) | The stack size for calculating cells recursively. Default value is 200. |
| [GetCharacterEncoding()](./getcharacterencoding/) | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [GetCustomEngine()](./getcustomengine/) | The custom formula calculation engine to extend the default calculation engine of [Aspose.Cells](../). |
| [GetIgnoreError()](./getignoreerror/) | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [GetLinkedDataSources()](./getlinkeddatasources/) | Specifies the data sources for external links used in formulas. |
| [GetPrecisionStrategy()](./getprecisionstrategy/) | Specifies the strategy for processing precision of calculation. |
| [GetRecursive()](./getrecursive/) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [GetRefreshDynamicArrayFormula()](./getrefreshdynamicarrayformula/) | Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [GetUserSpecifiedRefreshDynamicArrayFormula()](./getuserspecifiedrefreshdynamicarrayformula/) | Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CalculationOptions\& src)](./operator_asm/) | operator= |
| [SetCalcStackSize(int32_t value)](./setcalcstacksize/) | The stack size for calculating cells recursively. Default value is 200. |
| [SetCharacterEncoding(EncodingType value)](./setcharacterencoding/) | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [SetCustomEngine(AbstractCalculationEngine* value)](./setcustomengine/) | The custom formula calculation engine to extend the default calculation engine of [Aspose.Cells](../). |
| [SetIgnoreError(bool value)](./setignoreerror/) | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [SetLinkedDataSources(const Vector \<Workbook\>\& value)](./setlinkeddatasources/) | Specifies the data sources for external links used in formulas. |
| [SetPrecisionStrategy(CalculationPrecisionStrategy value)](./setprecisionstrategy/) | Specifies the strategy for processing precision of calculation. |
| [SetRecursive(bool value)](./setrecursive/) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [SetRefreshDynamicArrayFormula(bool value)](./setrefreshdynamicarrayformula/) | Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [~CalculationOptions()](./~calculationoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
