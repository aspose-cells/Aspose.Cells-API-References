---
title: "CalculationOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات الحساب."
type: docs
url: /ar/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

يمثل خيارات الحساب.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | حجم المكدس لحساب الخلايا بشكل متكرر. |
| [getCalculationMonitor()](#getCalculationMonitor--) | المراقب للمستخدم لتتبع تقدم حساب الصيغ. |
| [getCharacterEncoding()](#getCharacterEncoding--) | يحدد الترميز المستخدم لتشفير/فك تشفير الأحرف عند حساب الصيغ. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [getIgnoreError()](#getIgnoreError--) | يشير إلى ما إذا كان يجب تجاهل الأخطاء التي تم مواجهتها أثناء حساب الصيغ. |
| [getLinkedDataSources()](#getLinkedDataSources--) | يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | يحدد الاستراتيجية لمعالجة دقة الحساب. |
| [getRecursive()](#getRecursive--) | يشير إلى ما إذا كان يجب حساب الخلايا التابعة بشكل متكرر عند حساب خلية واحدة وتعتمد على خلايا أخرى. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | يشير إلى ما إذا كان المستخدم قد حدد صراحة سلوك تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ المحددة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | حجم المكدس لحساب الخلايا بشكل متكرر. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | المراقب للمستخدم لتتبع تقدم حساب الصيغ. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | يحدد الترميز المستخدم لتشفير/فك تشفير الأحرف عند حساب الصيغ. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | يشير إلى ما إذا كان يجب تجاهل الأخطاء التي تم مواجهتها أثناء حساب الصيغ. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | يحدد الاستراتيجية لمعالجة دقة الحساب. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | يشير إلى ما إذا كان يجب حساب الخلايا التابعة بشكل متكرر عند حساب خلية واحدة وتعتمد على خلايا أخرى. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


حجم المكدس لحساب الخلايا بشكل متكرر. القيمة الافتراضية هي 200.

**Remarks**

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


المراقب للمستخدم لتتبع تقدم حساب الصيغ.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ.

**Remarks**

مثل [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), هنا يمكنك تحديد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ التي سيتم حسابها، خاصة تلك المستخدمة في الدالة INDIRECT. بالنسبة لتلك الروابط الخارجية المستخدمة في الدالة INDIRECT، لا تُعتبر جزءًا من الروابط الخارجية لدفتر العمل ولا يمكن تحديثها بواسطة [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). يتم تحديد مطابقة تلك دفاتر العمل مع الروابط الخارجية بواسطة [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) و [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). لذا يرجى التأكد من أن [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) تم تحديده بالقيمة المناسبة (عادةً يجب أن تكون مماثلة لـ [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) لكل دفتر عمل حتى يمكن ربطها كما هو متوقع.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


يحدد الاستراتيجية لمعالجة دقة الحساب.

انظر [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ.

**Remarks**

إذا تم تحديد هذه الخاصية صراحةً، فستُستخدم القيمة المحددة لتحديد ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية. وإلا ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) غير صحيحة)، تعتمد القيمة الافتراضية عليها على نوع الصيغ التي تحتاج إلى حسابها: لحساب صيغ دفتر العمل، مثل [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-)، ستُعتبر هذه الخاصية true. في الحالات الأخرى، مثل [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) أو [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-)، ستُعتبر هذه الخاصية false.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


يشير إلى ما إذا كان المستخدم قد حدد صراحة سلوك تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ المحددة.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


حجم المكدس لحساب الخلايا بشكل متكرر. القيمة الافتراضية هي 200.

**Remarks**

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


المراقب للمستخدم لتتبع تقدم حساب الصيغ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ.

**Remarks**

مثل [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), هنا يمكنك تحديد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ التي سيتم حسابها، خاصة تلك المستخدمة في الدالة INDIRECT. بالنسبة لتلك الروابط الخارجية المستخدمة في الدالة INDIRECT، لا تُعتبر جزءًا من الروابط الخارجية لدفتر العمل ولا يمكن تحديثها بواسطة [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). يتم تحديد مطابقة تلك دفاتر العمل مع الروابط الخارجية بواسطة [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) و [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). لذا يرجى التأكد من أن [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) تم تحديده بالقيمة المناسبة (عادةً يجب أن تكون مماثلة لـ [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) لكل دفتر عمل حتى يمكن ربطها كما هو متوقع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


يحدد الاستراتيجية لمعالجة دقة الحساب.

انظر [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ.

**Remarks**

إذا تم تحديد هذه الخاصية صراحةً، فستُستخدم القيمة المحددة لتحديد ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية. وإلا ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) غير صحيحة)، تعتمد القيمة الافتراضية عليها على نوع الصيغ التي تحتاج إلى حسابها: لحساب صيغ دفتر العمل، مثل [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-)، ستُعتبر هذه الخاصية true. في الحالات الأخرى، مثل [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) أو [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-)، ستُعتبر هذه الخاصية false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

