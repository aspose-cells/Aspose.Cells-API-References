---
title: HeaderFooterCommand
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the command of header/footer
type: docs
url: /nodejs-cpp/headerfootercommand/
---

## HeaderFooterCommand class

Represents the command of header/footer

```javascript
class HeaderFooterCommand;
```


## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the header/footer' command type . |
| [getFont()](#getFont--)| Gets the font of the command's value. |
| [getText()](#getText--)| Gets the text of the command. |


### getType() {#getType--}

Gets the header/footer' command type .

```javascript
getType() : HeaderFooterCommandType;
```


**Returns**

[HeaderFooterCommandType](./headerfootercommandtype/)

### getFont() {#getFont--}

Gets the font of the command's value.

```javascript
getFont() : Font;
```


**Returns**

[Font](./font/)

**Remarks**

Useless for HeaderFooterCommandType.Picture.

### getText() {#getText--}

Gets the text of the command.

```javascript
getText() : string;
```


**Remarks**

Only valid for HeaderFooterCommandType.Text.


