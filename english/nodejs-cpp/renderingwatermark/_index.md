---
title: RenderingWatermark
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Watermark for rendering.
type: docs
url: /nodejs-cpp/renderingwatermark/
---

## RenderingWatermark class

Watermark for rendering.

```javascript
class RenderingWatermark;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(number[])](#constructor-numberarray-)| Creates instance of image watermark. |
| [constructor(string, RenderingFont)](#constructor-string-renderingfont-)| Creates instance of text watermark. |

## Methods

| Method | Description |
| --- | --- |
| [getRotation()](#getRotation--)| Gets or sets roation of the watermark in degrees. |
| [setRotation(number)](#setRotation-number-)| Gets or sets roation of the watermark in degrees. |
| [getScaleToPagePercent()](#getScaleToPagePercent--)| Gets or sets scale relative to target page in percent. |
| [setScaleToPagePercent(number)](#setScaleToPagePercent-number-)| Gets or sets scale relative to target page in percent. |
| [getOpacity()](#getOpacity--)| Gets or sets opacity of the watermark in range [0, 1]. |
| [setOpacity(number)](#setOpacity-number-)| Gets or sets opacity of the watermark in range [0, 1]. |
| [isBackground()](#isBackground--)| Indicates whether the watermark is placed behind page contents. |
| [setIsBackground(boolean)](#setIsBackground-boolean-)| Indicates whether the watermark is placed behind page contents. |
| [getText()](#getText--)| Gets text of the watermark. |
| [getFont()](#getFont--)| Gets font of the watermark. |
| [getImage()](#getImage--)| Gets image of the watermark. |
| [getHAlignment()](#getHAlignment--)| Gets or sets horizontal alignment of the watermark to the page. |
| [setHAlignment(TextAlignmentType)](#setHAlignment-textalignmenttype-)| Gets or sets horizontal alignment of the watermark to the page. |
| [getVAlignment()](#getVAlignment--)| Gets or sets vertical alignment of the watermark to the page. |
| [setVAlignment(TextAlignmentType)](#setVAlignment-textalignmenttype-)| Gets or sets vertical alignment of the watermark to the page. |
| [getOffsetX()](#getOffsetX--)| Gets or sets offset value to [HAlignment](../halignment/) |
| [setOffsetX(number)](#setOffsetX-number-)| Gets or sets offset value to [HAlignment](../halignment/) |
| [getOffsetY()](#getOffsetY--)| Gets or sets offset value to [VAlignment](../valignment/) |
| [setOffsetY(number)](#setOffsetY-number-)| Gets or sets offset value to [VAlignment](../valignment/) |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor(number[]) {#constructor-numberarray-}

Creates instance of image watermark.

```javascript
constructor(imageData: number[]);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageData | number[] |  |

### constructor(string, RenderingFont) {#constructor-string-renderingfont-}

Creates instance of text watermark.

```javascript
constructor(text: string, renderingFont: RenderingFont);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | watermark text |
| renderingFont | [RenderingFont](../renderingfont/) | watermark font |

### getRotation() {#getRotation--}

Gets or sets roation of the watermark in degrees.

```javascript
getRotation() : number;
```


### setRotation(number) {#setRotation-number-}

Gets or sets roation of the watermark in degrees.

```javascript
setRotation(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getScaleToPagePercent() {#getScaleToPagePercent--}

Gets or sets scale relative to target page in percent.

```javascript
getScaleToPagePercent() : number;
```


### setScaleToPagePercent(number) {#setScaleToPagePercent-number-}

Gets or sets scale relative to target page in percent.

```javascript
setScaleToPagePercent(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getOpacity() {#getOpacity--}

Gets or sets opacity of the watermark in range [0, 1].

```javascript
getOpacity() : number;
```


### setOpacity(number) {#setOpacity-number-}

Gets or sets opacity of the watermark in range [0, 1].

```javascript
setOpacity(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isBackground() {#isBackground--}

Indicates whether the watermark is placed behind page contents.

```javascript
isBackground() : boolean;
```


### setIsBackground(boolean) {#setIsBackground-boolean-}

Indicates whether the watermark is placed behind page contents.

```javascript
setIsBackground(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getText() {#getText--}

Gets text of the watermark.

```javascript
getText() : string;
```


### getFont() {#getFont--}

Gets font of the watermark.

```javascript
getFont() : RenderingFont;
```


**Returns**

[RenderingFont](../renderingfont/)

### getImage() {#getImage--}

Gets image of the watermark.

```javascript
getImage() : number[];
```


**Returns**

number[]

### getHAlignment() {#getHAlignment--}

Gets or sets horizontal alignment of the watermark to the page.

```javascript
getHAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

**Remarks**

Only Left, Center, Right is valid. Default is Left.

### setHAlignment(TextAlignmentType) {#setHAlignment-textalignmenttype-}

Gets or sets horizontal alignment of the watermark to the page.

```javascript
setHAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

**Remarks**

Only Left, Center, Right is valid. Default is Left.

### getVAlignment() {#getVAlignment--}

Gets or sets vertical alignment of the watermark to the page.

```javascript
getVAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](../textalignmenttype/)

**Remarks**

Only Top, Center, Bottom is valid. Default is Top.

### setVAlignment(TextAlignmentType) {#setVAlignment-textalignmenttype-}

Gets or sets vertical alignment of the watermark to the page.

```javascript
setVAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |

**Remarks**

Only Top, Center, Bottom is valid. Default is Top.

### getOffsetX() {#getOffsetX--}

Gets or sets offset value to [HAlignment](../halignment/)

```javascript
getOffsetX() : number;
```


### setOffsetX(number) {#setOffsetX-number-}

Gets or sets offset value to [HAlignment](../halignment/)

```javascript
setOffsetX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getOffsetY() {#getOffsetY--}

Gets or sets offset value to [VAlignment](../valignment/)

```javascript
getOffsetY() : number;
```


### setOffsetY(number) {#setOffsetY-number-}

Gets or sets offset value to [VAlignment](../valignment/)

```javascript
setOffsetY(value: number) : void;
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



