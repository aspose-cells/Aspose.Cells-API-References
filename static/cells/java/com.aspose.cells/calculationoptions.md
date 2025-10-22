##CalculationOptions
Represents options for calculation.
**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```
Represents options for calculation.
## Constructors
| Constructor | Description |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | The stack size for calculating cells recursively. |
| [getCalculationMonitor()](#getCalculationMonitor--) | The monitor for user to track the progress of formula calculation. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Specifies the encoding used for encoding/decoding characters when calculating formulas. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [getIgnoreError()](#getIgnoreError--) | Indicates whether errors encountered while calculating formulas should be ignored. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Specifies the data sources for external links used in formulas. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Specifies the strategy for processing precision of calculation. |
| [getRecursive()](#getRecursive--) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | The stack size for calculating cells recursively. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | The monitor for user to track the progress of formula calculation. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Specifies the encoding used for encoding/decoding characters when calculating formulas. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indicates whether errors encountered while calculating formulas should be ignored. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Specifies the data sources for external links used in formulas. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Specifies the strategy for processing precision of calculation. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```
The stack size for calculating cells recursively. Default value is 200.
**Remarks**
When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```
The monitor for user to track the progress of formula calculation.
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
The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.
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
Specifies the data sources for external links used in formulas.
**Remarks**
Like [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). The match of those workbooks with external links is determined by [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) and [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). So please make sure [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) for every workbook so they can be linked as expected.
**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```
Specifies the strategy for processing precision of calculation.
See [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).
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
Indicates whether dynamic array formulas should be refreshed before calculating formulas.
**Remarks**
If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), this property will be taken as true. For other cases, such as [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) or [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), this property will be taken as false.
**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```
Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas.
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
The stack size for calculating cells recursively. Default value is 200.
**Remarks**
When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```
The monitor for user to track the progress of formula calculation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |
### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```
Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |
### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```
The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |
### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```
Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```
Specifies the data sources for external links used in formulas.
**Remarks**
Like [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). The match of those workbooks with external links is determined by [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) and [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). So please make sure [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) for every workbook so they can be linked as expected.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |
### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```
Specifies the strategy for processing precision of calculation.
See [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```
Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```
Indicates whether dynamic array formulas should be refreshed before calculating formulas.
**Remarks**
If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), this property will be taken as true. For other cases, such as [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) or [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), this property will be taken as false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
