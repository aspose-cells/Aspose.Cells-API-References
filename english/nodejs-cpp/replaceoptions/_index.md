﻿---
title: ReplaceOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represent the replace options.
type: docs
url: /nodejs-cpp/replaceoptions/
---

## ReplaceOptions class

Represent the replace options.

```javascript
class ReplaceOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getCaseSensitive()](#getCaseSensitive--)| Indicates if the searched string is case sensitive. |
| [setCaseSensitive(boolean)](#setCaseSensitive-boolean-)| Indicates if the searched string is case sensitive. |
| [getMatchEntireCellContents()](#getMatchEntireCellContents--)| Indicates whether to match entire cells contents |
| [setMatchEntireCellContents(boolean)](#setMatchEntireCellContents-boolean-)| Indicates whether to match entire cells contents |
| [getRegexKey()](#getRegexKey--)| Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
| [setRegexKey(boolean)](#setRegexKey-boolean-)| Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
| [getFontSettings()](#getFontSettings--)| The rich formatted settings for the replaced text. |
| [setFontSettings(FontSetting[])](#setFontSettings-fontsettingarray-)| The rich formatted settings for the replaced text. |
| [getStyleFlags()](#getStyleFlags--)| Gets and sets flags of applying font settings. |
| [setStyleFlags(StyleFlag[])](#setStyleFlags-styleflagarray-)| Gets and sets flags of applying font settings. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getCaseSensitive() {#getCaseSensitive--}

Indicates if the searched string is case sensitive.

```javascript
getCaseSensitive() : boolean;
```


### setCaseSensitive(boolean) {#setCaseSensitive-boolean-}

Indicates if the searched string is case sensitive.

```javascript
setCaseSensitive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMatchEntireCellContents() {#getMatchEntireCellContents--}

Indicates whether to match entire cells contents

```javascript
getMatchEntireCellContents() : boolean;
```


**Remarks**

The default value is true.

### setMatchEntireCellContents(boolean) {#setMatchEntireCellContents-boolean-}

Indicates whether to match entire cells contents

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

Indicates whether the searched key is regex. If true then the searched key will be taken as regex.

```javascript
getRegexKey() : boolean;
```


### setRegexKey(boolean) {#setRegexKey-boolean-}

Indicates whether the searched key is regex. If true then the searched key will be taken as regex.

```javascript
setRegexKey(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFontSettings() {#getFontSettings--}

The rich formatted settings for the replaced text.

```javascript
getFontSettings() : FontSetting[];
```


**Returns**

[FontSetting](../fontsetting/)[]

### setFontSettings(FontSetting[]) {#setFontSettings-fontsettingarray-}

The rich formatted settings for the replaced text.

```javascript
setFontSettings(value: FontSetting[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontSetting](../fontsetting/)[] | The value to set. |

### getStyleFlags() {#getStyleFlags--}

Gets and sets flags of applying font settings.

```javascript
getStyleFlags() : StyleFlag[];
```


**Returns**

[StyleFlag](../styleflag/)[]

### setStyleFlags(StyleFlag[]) {#setStyleFlags-styleflagarray-}

Gets and sets flags of applying font settings.

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



