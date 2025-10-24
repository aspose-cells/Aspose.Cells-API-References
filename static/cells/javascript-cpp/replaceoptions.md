##ReplaceOptions
Represent the replace options.
## ReplaceOptions class
Represent the replace options.
```javascript
class ReplaceOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [caseSensitive](#caseSensitive--)| boolean | Indicates if the searched string is case sensitive. |
| [matchEntireCellContents](#matchEntireCellContents--)| boolean | Indicates whether to match entire cells contents |
| [regexKey](#regexKey--)| boolean | Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
| [fontSettings](#fontSettings--)| FontSetting[] | The rich formatted settings for the replaced text. |
| [styleFlags](#styleFlags--)| StyleFlag[] | Gets and sets flags of applying font settings. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### caseSensitive {#caseSensitive--}
Indicates if the searched string is case sensitive.
```javascript
caseSensitive : boolean;
```
### matchEntireCellContents {#matchEntireCellContents--}
Indicates whether to match entire cells contents
```javascript
matchEntireCellContents : boolean;
```
**Remarks**
The default value is true.
### regexKey {#regexKey--}
Indicates whether the searched key is regex. If true then the searched key will be taken as regex.
```javascript
regexKey : boolean;
```
### fontSettings {#fontSettings--}
The rich formatted settings for the replaced text.
```javascript
fontSettings : FontSetting[];
```
### styleFlags {#styleFlags--}
Gets and sets flags of applying font settings.
```javascript
styleFlags : StyleFlag[];
```
