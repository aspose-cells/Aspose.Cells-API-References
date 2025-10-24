##LowCodeMergeOptions
Options for merging multiple template files into one.
## LowCodeMergeOptions class
Options for merging multiple template files into one.
```javascript
class LowCodeMergeOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [saveOptions](#saveOptions--)| LowCodeSaveOptions | Save options for saving the split parts. |
| [loadOptionsProvider](#loadOptionsProvider--)| AbstractLowCodeLoadOptionsProvider | Provider of save options for saving the split parts. |
## Methods
| Method | Description |
| --- | --- |
| [getSaveOptions()](#getSaveOptions--)| <b>@deprecated.</b> Please use the 'saveOptions' property instead. Save options for saving the split parts. |
| [setSaveOptions(LowCodeSaveOptions)](#setSaveOptions-lowcodesaveoptions-)| <b>@deprecated.</b> Please use the 'saveOptions' property instead. Save options for saving the split parts. |
| [getLoadOptionsProvider()](#getLoadOptionsProvider--)| <b>@deprecated.</b> Please use the 'loadOptionsProvider' property instead. Provider of save options for saving the split parts. |
| [setLoadOptionsProvider(AbstractLowCodeLoadOptionsProvider)](#setLoadOptionsProvider-abstractlowcodeloadoptionsprovider-)| <b>@deprecated.</b> Please use the 'loadOptionsProvider' property instead. Provider of save options for saving the split parts. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### saveOptions {#saveOptions--}
Save options for saving the split parts.
```javascript
saveOptions : LowCodeSaveOptions;
```
### loadOptionsProvider {#loadOptionsProvider--}
Provider of save options for saving the split parts.
```javascript
loadOptionsProvider : AbstractLowCodeLoadOptionsProvider;
```
**Remarks**
If this property is specified, [LoadOptions](../loadoptions/) takes no effect because the output of every split part will be specified by the provider.
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
### getLoadOptionsProvider() {#getLoadOptionsProvider--}
```javascript
getLoadOptionsProvider() : AbstractLowCodeLoadOptionsProvider;
```
**Returns**
[AbstractLowCodeLoadOptionsProvider](../abstractlowcodeloadoptionsprovider/)
**Remarks**
If this property is specified, [LoadOptions](../loadoptions/) takes no effect because the output of every split part will be specified by the provider.
### setLoadOptionsProvider(AbstractLowCodeLoadOptionsProvider) {#setLoadOptionsProvider-abstractlowcodeloadoptionsprovider-}
```javascript
setLoadOptionsProvider(value: AbstractLowCodeLoadOptionsProvider) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractLowCodeLoadOptionsProvider](../abstractlowcodeloadoptionsprovider/) | The value to set. |
**Remarks**
If this property is specified, [LoadOptions](../loadoptions/) takes no effect because the output of every split part will be specified by the provider.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
