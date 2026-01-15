---
title: Aspose::Cells::FormulaSettings::SetEnableCalculationChain method
linktitle: SetEnableCalculationChain
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FormulaSettings::SetEnableCalculationChain method. Indicates whether to enable calculation chain for formulas. Default is false in C++.'
type: docs
weight: 2500
url: /cpp/aspose.cells/formulasettings/setenablecalculationchain/
---
## FormulaSettings::SetEnableCalculationChain method


Indicates whether to enable calculation chain for formulas. Default is false.

```cpp
void Aspose::Cells::FormulaSettings::SetEnableCalculationChain(bool value)
```

## Remarks


When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain. 
## See Also

* Class [Vector](../../vector/)
* Class [FormulaSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
