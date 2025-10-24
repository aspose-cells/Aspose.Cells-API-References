##LowCodeSplitOptions
Options for splitting spreadsheet.
## LowCodeSplitOptions class
Options for splitting spreadsheet.
```javascript
class LowCodeSplitOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [loadOptions](#loadOptions--)| LowCodeLoadOptions | Load options for loading the spreadsheet that will be split. |
| [saveOptions](#saveOptions--)| LowCodeSaveOptions | Save options for saving the split parts. |
| [saveOptionsProvider](#saveOptionsProvider--)| AbstractLowCodeSaveOptionsProvider | Provider of save options for saving the split parts. |
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
