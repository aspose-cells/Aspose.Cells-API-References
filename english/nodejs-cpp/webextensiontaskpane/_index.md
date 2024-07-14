---
title: WebExtensionTaskPane
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a persisted taskpane object.
type: docs
url: /nodejs-cpp/webextensiontaskpane/
---

## WebExtensionTaskPane class

Represents a persisted taskpane object.

```javascript
class WebExtensionTaskPane;
```


## Methods

| Method | Description |
| --- | --- |
| [getWebExtension()](#getWebExtension--)| Gets and sets the web extension part associated with the taskpane instance |
| [setWebExtension(WebExtension)](#setWebExtension-webextension-)| Gets and sets the web extension part associated with the taskpane instance |
| [getDockState()](#getDockState--)| Gets and sets the last-docked location of this taskpane object. |
| [setDockState(string)](#setDockState-string-)| Gets and sets the last-docked location of this taskpane object. |
| [isVisible()](#isVisible--)| Indicates whether the Task Pane shows as visible by default when the document opens. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Indicates whether the Task Pane shows as visible by default when the document opens. |
| [isLocked()](#isLocked--)| Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
| [getWidth()](#getWidth--)| Gets and sets the default width value for this taskpane instance. |
| [setWidth(number)](#setWidth-number-)| Gets and sets the default width value for this taskpane instance. |
| [getRow()](#getRow--)| Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |
| [setRow(number)](#setRow-number-)| Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |


### getWebExtension() {#getWebExtension--}

Gets and sets the web extension part associated with the taskpane instance

```javascript
getWebExtension() : WebExtension;
```


**Returns**

[WebExtension](/nodejs-cpp/webextension/)

### setWebExtension(WebExtension) {#setWebExtension-webextension-}

Gets and sets the web extension part associated with the taskpane instance

```javascript
setWebExtension(value: WebExtension) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebExtension](/nodejs-cpp/webextension/) | The value to set. |

### getDockState() {#getDockState--}

Gets and sets the last-docked location of this taskpane object.

```javascript
getDockState() : string;
```


### setDockState(string) {#setDockState-string-}

Gets and sets the last-docked location of this taskpane object.

```javascript
setDockState(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isVisible() {#isVisible--}

Indicates whether the Task Pane shows as visible by default when the document opens.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Indicates whether the Task Pane shows as visible by default when the document opens.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isLocked() {#isLocked--}

Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user.

```javascript
isLocked() : boolean;
```


### setIsLocked(boolean) {#setIsLocked-boolean-}

Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getWidth() {#getWidth--}

Gets and sets the default width value for this taskpane instance.

```javascript
getWidth() : number;
```


### setWidth(number) {#setWidth-number-}

Gets and sets the default width value for this taskpane instance.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRow() {#getRow--}

Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location.

```javascript
getRow() : number;
```


### setRow(number) {#setRow-number-}

Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location.

```javascript
setRow(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |


