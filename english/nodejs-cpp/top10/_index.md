---
title: Top10
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket as specified.
type: docs
url: /nodejs-cpp/top10/
---

## Top10 class

Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.

```javascript
class Top10;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [isPercent()](#isPercent--)| Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [setIsPercent(boolean)](#setIsPercent-boolean-)| Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [isBottom()](#isBottom--)| Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [setIsBottom(boolean)](#setIsBottom-boolean-)| Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [getRank()](#getRank--)| Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |
| [setRank(number)](#setRank-number-)| Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### isPercent() {#isPercent--}

Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false.

```javascript
isPercent() : boolean;
```


### setIsPercent(boolean) {#setIsPercent-boolean-}

Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false.

```javascript
setIsPercent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isBottom() {#isBottom--}

Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false.

```javascript
isBottom() : boolean;
```


### setIsBottom(boolean) {#setIsBottom-boolean-}

Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false.

```javascript
setIsBottom(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRank() {#getRank--}

Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10.

```javascript
getRank() : number;
```


### setRank(number) {#setRank-number-}

Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10.

```javascript
setRank(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |


