---
title: DrawObjectEventHandler
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Interface to get DrawObject and Bound when rendering.
type: docs
url: /nodejs-cpp/drawobjecteventhandler/
---

## DrawObjectEventHandler class

Interface to get DrawObject and Bound when rendering.

```javascript
abstract class DrawObjectEventHandler;
```


## Methods

| Method | Description |
| --- | --- |
| [draw(DrawObject, number, number, number, number)](#draw-drawobject-number-number-number-number-)| Implements this interface to get DrawObject and Bound when rendering. |


### draw(DrawObject, number, number, number, number) {#draw-drawobject-number-number-number-number-}

Implements this interface to get DrawObject and Bound when rendering.

```javascript
draw(drawObject: DrawObject, x: number, y: number, width: number, height: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| drawObject | [DrawObject](./drawobject/) | DrawObject will be initialized and returned when rendering |
| x | number | Left of DrawObject |
| y | number | Top of DrawObject |
| width | number | Width of DrawObject |
| height | number | Height of DrawObject |


