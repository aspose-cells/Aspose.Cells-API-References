##AutoFitterOptions
Represents all auto fitter options.
## AutoFitterOptions class
Represents all auto fitter options.
```javascript
class AutoFitterOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [defaultEditLanguage](#defaultEditLanguage--)| DefaultEditLanguage | Gets or sets default edit language. |
| [autoFitMergedCellsType](#autoFitMergedCellsType--)| AutoFitMergedCellsType | Gets and set the type of auto fitting row height of merged cells. |
| [onlyAuto](#onlyAuto--)| boolean | Indicates whether only fit the rows which height are not customed. |
| [ignoreHidden](#ignoreHidden--)| boolean | Ignores the hidden rows/columns. |
| [maxRowHeight](#maxRowHeight--)| number | Gets and sets the max row height(in unit of Point) when autofitting rows. |
| [autoFitWrappedTextType](#autoFitWrappedTextType--)| AutoFitWrappedTextType | Gets and sets the type of auto fitting wrapped text. |
| [formatStrategy](#formatStrategy--)| CellValueFormatStrategy | Gets and sets the formatted strategy. |
| [forRendering](#forRendering--)| boolean | Indicates whether fit for rendering purpose. |
## Methods
| Method | Description |
| --- | --- |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--)| <b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language. |
| [setDefaultEditLanguage(DefaultEditLanguage)](#setDefaultEditLanguage-defaulteditlanguage-)| <b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--)| <b>@deprecated.</b> Please use the 'autoFitMergedCellsType' property instead. Gets and set the type of auto fitting row height of merged cells. |
| [setAutoFitMergedCellsType(AutoFitMergedCellsType)](#setAutoFitMergedCellsType-autofitmergedcellstype-)| <b>@deprecated.</b> Please use the 'autoFitMergedCellsType' property instead. Gets and set the type of auto fitting row height of merged cells. |
| [getOnlyAuto()](#getOnlyAuto--)| <b>@deprecated.</b> Please use the 'onlyAuto' property instead. Indicates whether only fit the rows which height are not customed. |
| [setOnlyAuto(boolean)](#setOnlyAuto-boolean-)| <b>@deprecated.</b> Please use the 'onlyAuto' property instead. Indicates whether only fit the rows which height are not customed. |
| [getIgnoreHidden()](#getIgnoreHidden--)| <b>@deprecated.</b> Please use the 'ignoreHidden' property instead. Ignores the hidden rows/columns. |
| [setIgnoreHidden(boolean)](#setIgnoreHidden-boolean-)| <b>@deprecated.</b> Please use the 'ignoreHidden' property instead. Ignores the hidden rows/columns. |
| [getMaxRowHeight()](#getMaxRowHeight--)| <b>@deprecated.</b> Please use the 'maxRowHeight' property instead. Gets and sets the max row height(in unit of Point) when autofitting rows. |
| [setMaxRowHeight(number)](#setMaxRowHeight-number-)| <b>@deprecated.</b> Please use the 'maxRowHeight' property instead. Gets and sets the max row height(in unit of Point) when autofitting rows. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--)| <b>@deprecated.</b> Please use the 'autoFitWrappedTextType' property instead. Gets and sets the type of auto fitting wrapped text. |
| [setAutoFitWrappedTextType(AutoFitWrappedTextType)](#setAutoFitWrappedTextType-autofitwrappedtexttype-)| <b>@deprecated.</b> Please use the 'autoFitWrappedTextType' property instead. Gets and sets the type of auto fitting wrapped text. |
| [getFormatStrategy()](#getFormatStrategy--)| <b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the formatted strategy. |
| [setFormatStrategy(CellValueFormatStrategy)](#setFormatStrategy-cellvalueformatstrategy-)| <b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the formatted strategy. |
| [getForRendering()](#getForRendering--)| <b>@deprecated.</b> Please use the 'forRendering' property instead. Indicates whether fit for rendering purpose. |
| [setForRendering(boolean)](#setForRendering-boolean-)| <b>@deprecated.</b> Please use the 'forRendering' property instead. Indicates whether fit for rendering purpose. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### defaultEditLanguage {#defaultEditLanguage--}
Gets or sets default edit language.
```javascript
defaultEditLanguage : DefaultEditLanguage;
```
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).
### autoFitMergedCellsType {#autoFitMergedCellsType--}
Gets and set the type of auto fitting row height of merged cells.
```javascript
autoFitMergedCellsType : AutoFitMergedCellsType;
```
**Remarks**
Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.
### onlyAuto {#onlyAuto--}
Indicates whether only fit the rows which height are not customed.
```javascript
onlyAuto : boolean;
```
### ignoreHidden {#ignoreHidden--}
Ignores the hidden rows/columns.
```javascript
ignoreHidden : boolean;
```
### maxRowHeight {#maxRowHeight--}
Gets and sets the max row height(in unit of Point) when autofitting rows.
```javascript
maxRowHeight : number;
```
### autoFitWrappedTextType {#autoFitWrappedTextType--}
Gets and sets the type of auto fitting wrapped text.
```javascript
autoFitWrappedTextType : AutoFitWrappedTextType;
```
### formatStrategy {#formatStrategy--}
Gets and sets the formatted strategy.
```javascript
formatStrategy : CellValueFormatStrategy;
```
**Remarks**
The default value is CellStyle for performance.
### forRendering {#forRendering--}
Indicates whether fit for rendering purpose.
```javascript
forRendering : boolean;
```
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```javascript
getDefaultEditLanguage() : DefaultEditLanguage;
```
**Returns**
[DefaultEditLanguage](../defaulteditlanguage/)
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).
### setDefaultEditLanguage(DefaultEditLanguage) {#setDefaultEditLanguage-defaulteditlanguage-}
```javascript
setDefaultEditLanguage(value: DefaultEditLanguage) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DefaultEditLanguage](../defaulteditlanguage/) | The value to set. |
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```javascript
getAutoFitMergedCellsType() : AutoFitMergedCellsType;
```
**Returns**
[AutoFitMergedCellsType](../autofitmergedcellstype/)
**Remarks**
Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.
### setAutoFitMergedCellsType(AutoFitMergedCellsType) {#setAutoFitMergedCellsType-autofitmergedcellstype-}
```javascript
setAutoFitMergedCellsType(value: AutoFitMergedCellsType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitMergedCellsType](../autofitmergedcellstype/) | The value to set. |
**Remarks**
Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.
### getOnlyAuto() {#getOnlyAuto--}
```javascript
getOnlyAuto() : boolean;
```
### setOnlyAuto(boolean) {#setOnlyAuto-boolean-}
```javascript
setOnlyAuto(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIgnoreHidden() {#getIgnoreHidden--}
```javascript
getIgnoreHidden() : boolean;
```
### setIgnoreHidden(boolean) {#setIgnoreHidden-boolean-}
```javascript
setIgnoreHidden(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMaxRowHeight() {#getMaxRowHeight--}
```javascript
getMaxRowHeight() : number;
```
### setMaxRowHeight(number) {#setMaxRowHeight-number-}
```javascript
setMaxRowHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```javascript
getAutoFitWrappedTextType() : AutoFitWrappedTextType;
```
**Returns**
[AutoFitWrappedTextType](../autofitwrappedtexttype/)
### setAutoFitWrappedTextType(AutoFitWrappedTextType) {#setAutoFitWrappedTextType-autofitwrappedtexttype-}
```javascript
setAutoFitWrappedTextType(value: AutoFitWrappedTextType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitWrappedTextType](../autofitwrappedtexttype/) | The value to set. |
### getFormatStrategy() {#getFormatStrategy--}
```javascript
getFormatStrategy() : CellValueFormatStrategy;
```
**Returns**
[CellValueFormatStrategy](../cellvalueformatstrategy/)
**Remarks**
The default value is CellStyle for performance.
### setFormatStrategy(CellValueFormatStrategy) {#setFormatStrategy-cellvalueformatstrategy-}
```javascript
setFormatStrategy(value: CellValueFormatStrategy) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellValueFormatStrategy](../cellvalueformatstrategy/) | The value to set. |
**Remarks**
The default value is CellStyle for performance.
### getForRendering() {#getForRendering--}
```javascript
getForRendering() : boolean;
```
### setForRendering(boolean) {#setForRendering-boolean-}
```javascript
setForRendering(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
