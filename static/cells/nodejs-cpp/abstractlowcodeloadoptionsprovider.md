##AbstractLowCodeLoadOptionsProvider
Implementation to provide multiple load options for processes that use multiple inputssuch as template files.
## AbstractLowCodeLoadOptionsProvider class
Implementation to provide multiple load options for processes that use multiple inputs(such as template files).
```javascript
class AbstractLowCodeLoadOptionsProvider;
```
### Remarks
For example, [SpreadsheetMerger](../spreadsheetmerger/) feature requires multiple template files to merge.
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getCurrent()](#getCurrent--)| Gets the load options from which to load data of currently processed part. |
| [moveNext()](#moveNext--)| Checks whether there is more input. |
| [finish(LowCodeLoadOptions)](#finish-lowcodeloadoptions-)| Releases resources after processing currently part of input. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getCurrent() {#getCurrent--}
Gets the load options from which to load data of currently processed part.
```javascript
getCurrent() : LowCodeLoadOptions;
```
**Returns**
[LowCodeLoadOptions](../lowcodeloadoptions/)
### moveNext() {#moveNext--}
Checks whether there is more input.
```javascript
moveNext() : boolean;
```
### finish(LowCodeLoadOptions) {#finish-lowcodeloadoptions-}
Releases resources after processing currently part of input.
```javascript
finish(part: LowCodeLoadOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../lowcodeloadoptions/) | the load options used for currently split part. |
**Remarks**
By default this method just closes the stream specified by the [LowCodeLoadOptions.InputStream](../lowcodeloadoptions.inputstream/) directly(if the load options specified a Stream as source). User may overwrite this method to control how to release resources according to their requirement and the implementation of [Current](../current/).
