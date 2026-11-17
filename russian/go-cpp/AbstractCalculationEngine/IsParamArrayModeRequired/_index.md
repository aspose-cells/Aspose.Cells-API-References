---
title: "IsParamArrayModeRequired Метод"
linktitle: "IsParamArrayModeRequired"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "IsParamArrayModeRequired метод. Инкапсулирует функцию, представляющую isparamarraymoderequired в Go."
type: docs
weight: 200
url: /ru/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

Указывает, требуется ли этому движку вычислять параметр в режиме массива. Значение по умолчанию — false.Если CalculationData.GetParamValueInArrayMode(int, int, int) требуется при вычислении customfunctions и пользователь не обновил их определение (через Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), это свойство должно быть установлено в true.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## Примечания


## См. также

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
