---
title: ICustomFunction
second_title: Aspose.Cells for Java API Reference
description: Allows users to add their custom formula calculation functions to extend the calculation engine.
type: docs
weight: 674
url: /java/com.aspose.cells/icustomfunction/
---
```
public interface ICustomFunction
```

Allows users to add their custom formula calculation functions to extend the calculation engine. User should not modify any part in the Workbook directly in this implementation. Otherwise unexpected result or Exception may be caused. NOTE: This member is now obsolete. Instead, please use AbstractCalculationEngine which provides more convenient and flexible APIs for manipulating custom functions. This interface will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.
## Methods

| Method | Description |
| --- | --- |
| [calculateCustomFunction(String functionName, ArrayList paramsList, ArrayList contextObjects)](#calculateCustomFunction-java.lang.String-java.util.ArrayList-java.util.ArrayList-) | Calculates the result of custom function. |
### calculateCustomFunction(String functionName, ArrayList paramsList, ArrayList contextObjects) {#calculateCustomFunction-java.lang.String-java.util.ArrayList-java.util.ArrayList-}
```
public abstract Object calculateCustomFunction(String functionName, ArrayList paramsList, ArrayList contextObjects)
```


Calculates the result of custom function. Currently there are 3 fixed context objects and some varialbe context objects:

1. Current Workbook object.

2. Current Worksheet object.

3. Current Cell object.

Others are custom function parameters text.

If a custom function name is not supported, please return a null reference.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionName | java.lang.String | InnerCustom function name, such as "MyFunc1". |
| paramsList | java.util.ArrayList | A list of parameters value for custom functions. |
| contextObjects | java.util.ArrayList | A list of context objects. |

**Returns:**
java.lang.Object - Result of custom function.
