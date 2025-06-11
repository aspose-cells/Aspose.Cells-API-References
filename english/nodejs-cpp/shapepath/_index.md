---
title: ShapePath
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a creation path consisting of a series of moves lines and curves that when combined will form a geometric shape.
type: docs
url: /nodejs-cpp/shapepath/
---

## ShapePath class

Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.

```javascript
class ShapePath;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Initializes a new instance of the [ShapePath](../shapepath/) class. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [pathSegementList](#pathSegementList--)| ShapeSegmentPathCollection | Readonly. Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list |

## Methods

| Method | Description |
| --- | --- |
| [getPathSegementList()](#getPathSegementList--)| <b>@deprecated.</b> Please use the 'pathSegementList' property instead. Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list |
| [moveTo(number, number)](#moveTo-number-number-)| Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure. |
| [lineTo(number, number)](#lineTo-number-number-)| Appends a line segment to the current figure. The starting point is the end point of the current figure. |
| [cubicBezierTo(number, number, number, number, number, number)](#cubicBezierTo-number-number-number-number-number-number-)| Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure. |
| [arcTo(number, number, number, number)](#arcTo-number-number-number-number-)| Appends an elliptical arc to the current figure. The starting point is the end point of the current figure. |
| [close()](#close--)| Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Initializes a new instance of the [ShapePath](../shapepath/) class.

```javascript
constructor();
```


### pathSegementList {#pathSegementList--}

Readonly. Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list

```javascript
pathSegementList : ShapeSegmentPathCollection;
```


### getPathSegementList() {#getPathSegementList--}

<b>@deprecated.</b> Please use the 'pathSegementList' property instead. Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list

```javascript
getPathSegementList() : ShapeSegmentPathCollection;
```


**Returns**

[ShapeSegmentPathCollection](../shapesegmentpathcollection/)

### moveTo(number, number) {#moveTo-number-number-}

Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.

```javascript
moveTo(x: number, y: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | number | The x-coordinate of the starting point of the figure. |
| y | number | The y-coordinate of the starting point of the figure. |

### lineTo(number, number) {#lineTo-number-number-}

Appends a line segment to the current figure. The starting point is the end point of the current figure.

```javascript
lineTo(x: number, y: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | number | The x-coordinate of the endpoint of the line segment. |
| y | number | The y-coordinate of the endpoint of the line segment. |

### cubicBezierTo(number, number, number, number, number, number) {#cubicBezierTo-number-number-number-number-number-number-}

Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.

```javascript
cubicBezierTo(ctrX1: number, ctrY1: number, ctrX2: number, ctrY2: number, endX: number, endY: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ctrX1 | number | The x-coordinate of the first control point for the curve. |
| ctrY1 | number | The y-coordinate of the first control point for the curve. |
| ctrX2 | number | The x-coordinate of the second control point for the curve. |
| ctrY2 | number | The y-coordinate of the second control point for the curve. |
| endX | number | The x-coordinate of the endpoint of the curve. |
| endY | number | The y-coordinate of the endpoint of the curve. |

### arcTo(number, number, number, number) {#arcTo-number-number-number-number-}

Appends an elliptical arc to the current figure. The starting point is the end point of the current figure.

```javascript
arcTo(wR: number, hR: number, stAng: number, swAng: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| wR | number | The half-width of the rectangular area of ​​the ellipse that draws the arc. |
| hR | number | The half-height of the rectangular area of ​​the ellipse that draws the arc. |
| stAng | number | The starting angle of the arc, measured in degrees clockwise from the x-axis. |
| swAng | number | The angle between startAngle and the end of the arc. |

### close() {#close--}

Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point.

```javascript
close() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



