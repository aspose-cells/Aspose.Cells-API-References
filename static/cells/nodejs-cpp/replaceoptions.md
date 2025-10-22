##ReplaceOptions
Represent the replace options.
## ReplaceOptions class
Represent the replace options.
```javascript
class ReplaceOptions;
```
## Constructors
| Constructor | Description |
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
## Methods
| Method | Description |
| --- | --- |
| [getCaseSensitive()](#getCaseSensitive--)| <b>@deprecated.</b> Please use the 'caseSensitive' property instead. Indicates if the searched string is case sensitive. |
| [setCaseSensitive(boolean)](#setCaseSensitive-boolean-)| <b>@deprecated.</b> Please use the 'caseSensitive' property instead. Indicates if the searched string is case sensitive. |
| [getMatchEntireCellContents()](#getMatchEntireCellContents--)| <b>@deprecated.</b> Please use the 'matchEntireCellContents' property instead. Indicates whether to match entire cells contents |
| [setMatchEntireCellContents(boolean)](#setMatchEntireCellContents-boolean-)| <b>@deprecated.</b> Please use the 'matchEntireCellContents' property instead. Indicates whether to match entire cells contents |
| [getRegexKey()](#getRegexKey--)| <b>@deprecated.</b> Please use the 'regexKey' property instead. Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
| [setRegexKey(boolean)](#setRegexKey-boolean-)| <b>@deprecated.</b> Please use the 'regexKey' property instead. Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
| [getFontSettings()](#getFontSettings--)| <b>@deprecated.</b> Please use the 'fontSettings' property instead. The rich formatted settings for the replaced text. |
| [setFontSettings(FontSetting[])](#setFontSettings-fontsettingarray-)| <b>@deprecated.</b> Please use the 'fontSettings' property instead. The rich formatted settings for the replaced text. |
| [getStyleFlags()](#getStyleFlags--)| <b>@deprecated.</b> Please use the 'styleFlags' property instead. Gets and sets flags of applying font settings. |
| [setStyleFlags(StyleFlag[])](#setStyleFlags-styleflagarray-)| <b>@deprecated.</b> Please use the 'styleFlags' property instead. Gets and sets flags of applying font settings. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getCaseSensitive() {#getCaseSensitive--}
```javascript
getCaseSensitive() : boolean;
```
### setCaseSensitive(boolean) {#setCaseSensitive-boolean-}
```javascript
setCaseSensitive(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMatchEntireCellContents() {#getMatchEntireCellContents--}
```javascript
getMatchEntireCellContents() : boolean;
```
**Remarks**
The default value is true.
### setMatchEntireCellContents(boolean) {#setMatchEntireCellContents-boolean-}
```javascript
setMatchEntireCellContents(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is true.
### getRegexKey() {#getRegexKey--}
```javascript
getRegexKey() : boolean;
```
### setRegexKey(boolean) {#setRegexKey-boolean-}
```javascript
setRegexKey(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFontSettings() {#getFontSettings--}
```javascript
getFontSettings() : FontSetting[];
```
**Returns**
[FontSetting](../fontsetting/)[]
### setFontSettings(FontSetting[]) {#setFontSettings-fontsettingarray-}
```javascript
setFontSettings(value: FontSetting[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontSetting](../fontsetting/)[] | The value to set. |
### getStyleFlags() {#getStyleFlags--}
```javascript
getStyleFlags() : StyleFlag[];
```
**Returns**
[StyleFlag](../styleflag/)[]
### setStyleFlags(StyleFlag[]) {#setStyleFlags-styleflagarray-}
```javascript
setStyleFlags(value: StyleFlag[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [StyleFlag](../styleflag/)[] | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
