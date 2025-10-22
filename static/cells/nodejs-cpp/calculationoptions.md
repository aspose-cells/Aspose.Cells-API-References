##CalculationOptions
Represents options for calculation.
## CalculationOptions class
Represents options for calculation.
```javascript
class CalculationOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [ignoreError](#ignoreError--)| boolean | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [recursive](#recursive--)| boolean | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [userSpecifiedRefreshDynamicArrayFormula](#userSpecifiedRefreshDynamicArrayFormula--)| boolean | Readonly. Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas. |
| [refreshDynamicArrayFormula](#refreshDynamicArrayFormula--)| boolean | Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [customEngine](#customEngine--)| AbstractCalculationEngine | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [calcStackSize](#calcStackSize--)| number | The stack size for calculating cells recursively. Default value is 200. |
| [precisionStrategy](#precisionStrategy--)| CalculationPrecisionStrategy | Specifies the strategy for processing precision of calculation. |
| [linkedDataSources](#linkedDataSources--)| Workbook[] | Specifies the data sources for external links used in formulas. |
| [characterEncoding](#characterEncoding--)| EncodingType | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
## Methods
| Method | Description |
| --- | --- |
| [getIgnoreError()](#getIgnoreError--)| <b>@deprecated.</b> Please use the 'ignoreError' property instead. Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [setIgnoreError(boolean)](#setIgnoreError-boolean-)| <b>@deprecated.</b> Please use the 'ignoreError' property instead. Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [getRecursive()](#getRecursive--)| <b>@deprecated.</b> Please use the 'recursive' property instead. Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [setRecursive(boolean)](#setRecursive-boolean-)| <b>@deprecated.</b> Please use the 'recursive' property instead. Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--)| <b>@deprecated.</b> Please use the 'userSpecifiedRefreshDynamicArrayFormula' property instead. Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--)| <b>@deprecated.</b> Please use the 'refreshDynamicArrayFormula' property instead. Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [setRefreshDynamicArrayFormula(boolean)](#setRefreshDynamicArrayFormula-boolean-)| <b>@deprecated.</b> Please use the 'refreshDynamicArrayFormula' property instead. Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [getCustomEngine()](#getCustomEngine--)| <b>@deprecated.</b> Please use the 'customEngine' property instead. The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [setCustomEngine(AbstractCalculationEngine)](#setCustomEngine-abstractcalculationengine-)| <b>@deprecated.</b> Please use the 'customEngine' property instead. The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [getCalcStackSize()](#getCalcStackSize--)| <b>@deprecated.</b> Please use the 'calcStackSize' property instead. The stack size for calculating cells recursively. Default value is 200. |
| [setCalcStackSize(number)](#setCalcStackSize-number-)| <b>@deprecated.</b> Please use the 'calcStackSize' property instead. The stack size for calculating cells recursively. Default value is 200. |
| [getPrecisionStrategy()](#getPrecisionStrategy--)| <b>@deprecated.</b> Please use the 'precisionStrategy' property instead. Specifies the strategy for processing precision of calculation. |
| [setPrecisionStrategy(CalculationPrecisionStrategy)](#setPrecisionStrategy-calculationprecisionstrategy-)| <b>@deprecated.</b> Please use the 'precisionStrategy' property instead. Specifies the strategy for processing precision of calculation. |
| [getLinkedDataSources()](#getLinkedDataSources--)| <b>@deprecated.</b> Please use the 'linkedDataSources' property instead. Specifies the data sources for external links used in formulas. |
| [setLinkedDataSources(Workbook[])](#setLinkedDataSources-workbookarray-)| <b>@deprecated.</b> Please use the 'linkedDataSources' property instead. Specifies the data sources for external links used in formulas. |
| [getCharacterEncoding()](#getCharacterEncoding--)| <b>@deprecated.</b> Please use the 'characterEncoding' property instead. Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [setCharacterEncoding(EncodingType)](#setCharacterEncoding-encodingtype-)| <b>@deprecated.</b> Please use the 'characterEncoding' property instead. Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### ignoreError {#ignoreError--}
Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.
```javascript
ignoreError : boolean;
```
### recursive {#recursive--}
Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.
```javascript
recursive : boolean;
```
### userSpecifiedRefreshDynamicArrayFormula {#userSpecifiedRefreshDynamicArrayFormula--}
Readonly. Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas.
```javascript
userSpecifiedRefreshDynamicArrayFormula : boolean;
```
### refreshDynamicArrayFormula {#refreshDynamicArrayFormula--}
Indicates whether dynamic array formulas should be refreshed before calculating formulas.
```javascript
refreshDynamicArrayFormula : boolean;
```
**Remarks**
If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([UserSpecifiedRefreshDynamicArrayFormula](../userspecifiedrefreshdynamicarrayformula/) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.CalculateFormula(CalculationOptions)](../workbook.calculateformula(calculationoptions)/), this property will be taken as true. For other cases, such as [Cell.Calculate(CalculationOptions)](../cell.calculate(calculationoptions)/) or [Worksheet.CalculateFormula(CalculationOptions, bool)](../worksheet.calculateformula(calculationoptions, bool)/), this property will be taken as false.
### customEngine {#customEngine--}
The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.
```javascript
customEngine : AbstractCalculationEngine;
```
### calcStackSize {#calcStackSize--}
The stack size for calculating cells recursively. Default value is 200.
```javascript
calcStackSize : number;
```
**Remarks**
When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
### precisionStrategy {#precisionStrategy--}
Specifies the strategy for processing precision of calculation.
```javascript
precisionStrategy : CalculationPrecisionStrategy;
```
### linkedDataSources {#linkedDataSources--}
Specifies the data sources for external links used in formulas.
```javascript
linkedDataSources : Workbook[];
```
**Remarks**
Like [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/). The match of those workbooks with external links is determined by [Workbook.FileName](../workbook.filename/) and [ExternalLink.DataSource](../externallink.datasource/). So please make sure [Workbook.FileName](../workbook.filename/) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.DataSource](../externallink.datasource/)) for every workbook so they can be linked as expected.
### characterEncoding {#characterEncoding--}
Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.
```javascript
characterEncoding : EncodingType;
```
### getIgnoreError() {#getIgnoreError--}
```javascript
getIgnoreError() : boolean;
```
### setIgnoreError(boolean) {#setIgnoreError-boolean-}
```javascript
setIgnoreError(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRecursive() {#getRecursive--}
```javascript
getRecursive() : boolean;
```
### setRecursive(boolean) {#setRecursive-boolean-}
```javascript
setRecursive(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```javascript
getUserSpecifiedRefreshDynamicArrayFormula() : boolean;
```
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```javascript
getRefreshDynamicArrayFormula() : boolean;
```
**Remarks**
If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([UserSpecifiedRefreshDynamicArrayFormula](../userspecifiedrefreshdynamicarrayformula/) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.CalculateFormula(CalculationOptions)](../workbook.calculateformula(calculationoptions)/), this property will be taken as true. For other cases, such as [Cell.Calculate(CalculationOptions)](../cell.calculate(calculationoptions)/) or [Worksheet.CalculateFormula(CalculationOptions, bool)](../worksheet.calculateformula(calculationoptions, bool)/), this property will be taken as false.
### setRefreshDynamicArrayFormula(boolean) {#setRefreshDynamicArrayFormula-boolean-}
```javascript
setRefreshDynamicArrayFormula(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([UserSpecifiedRefreshDynamicArrayFormula](../userspecifiedrefreshdynamicarrayformula/) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.CalculateFormula(CalculationOptions)](../workbook.calculateformula(calculationoptions)/), this property will be taken as true. For other cases, such as [Cell.Calculate(CalculationOptions)](../cell.calculate(calculationoptions)/) or [Worksheet.CalculateFormula(CalculationOptions, bool)](../worksheet.calculateformula(calculationoptions, bool)/), this property will be taken as false.
### getCustomEngine() {#getCustomEngine--}
```javascript
getCustomEngine() : AbstractCalculationEngine;
```
**Returns**
[AbstractCalculationEngine](../abstractcalculationengine/)
### setCustomEngine(AbstractCalculationEngine) {#setCustomEngine-abstractcalculationengine-}
```javascript
setCustomEngine(value: AbstractCalculationEngine) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../abstractcalculationengine/) | The value to set. |
### getCalcStackSize() {#getCalcStackSize--}
```javascript
getCalcStackSize() : number;
```
**Remarks**
When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
### setCalcStackSize(number) {#setCalcStackSize-number-}
```javascript
setCalcStackSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
### getPrecisionStrategy() {#getPrecisionStrategy--}
```javascript
getPrecisionStrategy() : CalculationPrecisionStrategy;
```
**Returns**
[CalculationPrecisionStrategy](../calculationprecisionstrategy/)
### setPrecisionStrategy(CalculationPrecisionStrategy) {#setPrecisionStrategy-calculationprecisionstrategy-}
```javascript
setPrecisionStrategy(value: CalculationPrecisionStrategy) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CalculationPrecisionStrategy](../calculationprecisionstrategy/) | The value to set. |
### getLinkedDataSources() {#getLinkedDataSources--}
```javascript
getLinkedDataSources() : Workbook[];
```
**Returns**
[Workbook](../workbook/)[]
**Remarks**
Like [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/). The match of those workbooks with external links is determined by [Workbook.FileName](../workbook.filename/) and [ExternalLink.DataSource](../externallink.datasource/). So please make sure [Workbook.FileName](../workbook.filename/) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.DataSource](../externallink.datasource/)) for every workbook so they can be linked as expected.
### setLinkedDataSources(Workbook[]) {#setLinkedDataSources-workbookarray-}
```javascript
setLinkedDataSources(value: Workbook[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Workbook](../workbook/)[] | The value to set. |
**Remarks**
Like [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/). The match of those workbooks with external links is determined by [Workbook.FileName](../workbook.filename/) and [ExternalLink.DataSource](../externallink.datasource/). So please make sure [Workbook.FileName](../workbook.filename/) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.DataSource](../externallink.datasource/)) for every workbook so they can be linked as expected.
### getCharacterEncoding() {#getCharacterEncoding--}
```javascript
getCharacterEncoding() : EncodingType;
```
**Returns**
[EncodingType](../encodingtype/)
### setCharacterEncoding(EncodingType) {#setCharacterEncoding-encodingtype-}
```javascript
setCharacterEncoding(value: EncodingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
