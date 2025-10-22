##LowCodeSplitOptions
Options for splitting spreadsheet.
## LowCodeSplitOptions class
Options for splitting spreadsheet.
```javascript
class LowCodeSplitOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [loadOptions](#loadOptions--)| LowCodeLoadOptions | Load options for loading the spreadsheet that will be split. |
| [saveOptions](#saveOptions--)| LowCodeSaveOptions | Save options for saving the split parts. |
| [saveOptionsProvider](#saveOptionsProvider--)| AbstractLowCodeSaveOptionsProvider | Provider of save options for saving the split parts. |
## Methods
| Method | Description |
| --- | --- |
| [getLoadOptions()](#getLoadOptions--)| <b>@deprecated.</b> Please use the 'loadOptions' property instead. Load options for loading the spreadsheet that will be split. |
| [setLoadOptions(LowCodeLoadOptions)](#setLoadOptions-lowcodeloadoptions-)| <b>@deprecated.</b> Please use the 'loadOptions' property instead. Load options for loading the spreadsheet that will be split. |
| [getSaveOptions()](#getSaveOptions--)| <b>@deprecated.</b> Please use the 'saveOptions' property instead. Save options for saving the split parts. |
| [setSaveOptions(LowCodeSaveOptions)](#setSaveOptions-lowcodesaveoptions-)| <b>@deprecated.</b> Please use the 'saveOptions' property instead. Save options for saving the split parts. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--)| <b>@deprecated.</b> Please use the 'saveOptionsProvider' property instead. Provider of save options for saving the split parts. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider)](#setSaveOptionsProvider-abstractlowcodesaveoptionsprovider-)| <b>@deprecated.</b> Please use the 'saveOptionsProvider' property instead. Provider of save options for saving the split parts. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### loadOptions {#loadOptions--}
Load options for loading the spreadsheet that will be split.
```javascript
loadOptions : LowCodeLoadOptions;
```
### saveOptions {#saveOptions--}
Save options for saving the split parts.
```javascript
saveOptions : LowCodeSaveOptions;
```
### saveOptionsProvider {#saveOptionsProvider--}
Provider of save options for saving the split parts.
```javascript
saveOptionsProvider : AbstractLowCodeSaveOptionsProvider;
```
**Remarks**
If this property is specified, [SaveOptions](../saveoptions/) takes no effect because the output of every split part will be specified by the provider.
### getLoadOptions() {#getLoadOptions--}
```javascript
getLoadOptions() : LowCodeLoadOptions;
```
**Returns**
[LowCodeLoadOptions](../lowcodeloadoptions/)
### setLoadOptions(LowCodeLoadOptions) {#setLoadOptions-lowcodeloadoptions-}
```javascript
setLoadOptions(value: LowCodeLoadOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LowCodeLoadOptions](../lowcodeloadoptions/) | The value to set. |
### getSaveOptions() {#getSaveOptions--}
```javascript
getSaveOptions() : LowCodeSaveOptions;
```
**Returns**
[LowCodeSaveOptions](../lowcodesaveoptions/)
### setSaveOptions(LowCodeSaveOptions) {#setSaveOptions-lowcodesaveoptions-}
```javascript
setSaveOptions(value: LowCodeSaveOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../lowcodesaveoptions/) | The value to set. |
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```javascript
getSaveOptionsProvider() : AbstractLowCodeSaveOptionsProvider;
```
**Returns**
[AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
**Remarks**
If this property is specified, [SaveOptions](../saveoptions/) takes no effect because the output of every split part will be specified by the provider.
### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider) {#setSaveOptionsProvider-abstractlowcodesaveoptionsprovider-}
```javascript
setSaveOptionsProvider(value: AbstractLowCodeSaveOptionsProvider) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/) | The value to set. |
**Remarks**
If this property is specified, [SaveOptions](../saveoptions/) takes no effect because the output of every split part will be specified by the provider.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
