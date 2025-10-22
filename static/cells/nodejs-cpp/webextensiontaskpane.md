##WebExtensionTaskPane
Represents a persisted taskpane object.
## WebExtensionTaskPane class
Represents a persisted taskpane object.
```javascript
class WebExtensionTaskPane;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [webExtension](#webExtension--)| WebExtension | Gets and sets the web extension part associated with the taskpane instance |
| [dockState](#dockState--)| string | Gets and sets the last-docked location of this taskpane object. |
| [isVisible](#isVisible--)| boolean | Indicates whether the Task Pane shows as visible by default when the document opens. |
| [isLocked](#isLocked--)| boolean | Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
| [width](#width--)| number | Gets and sets the default width value for this taskpane instance. |
| [row](#row--)| number | Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |
## Methods
| Method | Description |
| --- | --- |
| [getWebExtension()](#getWebExtension--)| <b>@deprecated.</b> Please use the 'webExtension' property instead. Gets and sets the web extension part associated with the taskpane instance |
| [setWebExtension(WebExtension)](#setWebExtension-webextension-)| <b>@deprecated.</b> Please use the 'webExtension' property instead. Gets and sets the web extension part associated with the taskpane instance |
| [getDockState()](#getDockState--)| <b>@deprecated.</b> Please use the 'dockState' property instead. Gets and sets the last-docked location of this taskpane object. |
| [setDockState(string)](#setDockState-string-)| <b>@deprecated.</b> Please use the 'dockState' property instead. Gets and sets the last-docked location of this taskpane object. |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Indicates whether the Task Pane shows as visible by default when the document opens. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Indicates whether the Task Pane shows as visible by default when the document opens. |
| [isLocked()](#isLocked--)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
| [getWidth()](#getWidth--)| <b>@deprecated.</b> Please use the 'width' property instead. Gets and sets the default width value for this taskpane instance. |
| [setWidth(number)](#setWidth-number-)| <b>@deprecated.</b> Please use the 'width' property instead. Gets and sets the default width value for this taskpane instance. |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |
| [setRow(number)](#setRow-number-)| <b>@deprecated.</b> Please use the 'row' property instead. Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### webExtension {#webExtension--}
Gets and sets the web extension part associated with the taskpane instance
```javascript
webExtension : WebExtension;
```
### dockState {#dockState--}
Gets and sets the last-docked location of this taskpane object.
```javascript
dockState : string;
```
### isVisible {#isVisible--}
Indicates whether the Task Pane shows as visible by default when the document opens.
```javascript
isVisible : boolean;
```
### isLocked {#isLocked--}
Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user.
```javascript
isLocked : boolean;
```
### width {#width--}
Gets and sets the default width value for this taskpane instance.
```javascript
width : number;
```
### row {#row--}
Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location.
```javascript
row : number;
```
### getWebExtension() {#getWebExtension--}
```javascript
getWebExtension() : WebExtension;
```
**Returns**
[WebExtension](../webextension/)
### setWebExtension(WebExtension) {#setWebExtension-webextension-}
```javascript
setWebExtension(value: WebExtension) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebExtension](../webextension/) | The value to set. |
### getDockState() {#getDockState--}
```javascript
getDockState() : string;
```
### setDockState(string) {#setDockState-string-}
```javascript
setDockState(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isVisible() {#isVisible--}
```javascript
isVisible() : boolean;
```
### setIsVisible(boolean) {#setIsVisible-boolean-}
```javascript
setIsVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isLocked() {#isLocked--}
```javascript
isLocked() : boolean;
```
### setIsLocked(boolean) {#setIsLocked-boolean-}
```javascript
setIsLocked(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getWidth() {#getWidth--}
```javascript
getWidth() : number;
```
### setWidth(number) {#setWidth-number-}
```javascript
setWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### setRow(number) {#setRow-number-}
```javascript
setRow(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
