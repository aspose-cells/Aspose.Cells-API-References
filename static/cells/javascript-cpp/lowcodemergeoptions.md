##LowCodeMergeOptions
Options for merging multiple template files into one.
## LowCodeMergeOptions class
Options for merging multiple template files into one.
```javascript
class LowCodeMergeOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [saveOptions](#saveOptions--)| LowCodeSaveOptions | Save options for saving the split parts. |
| [loadOptionsProvider](#loadOptionsProvider--)| AbstractLowCodeLoadOptionsProvider | Provider of save options for saving the split parts. |
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
