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
