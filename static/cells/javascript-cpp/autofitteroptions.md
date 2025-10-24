##AutoFitterOptions
Represents all auto fitter options.
## AutoFitterOptions class
Represents all auto fitter options.
```javascript
class AutoFitterOptions;
```
## Constructors
| Name | Description |
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
