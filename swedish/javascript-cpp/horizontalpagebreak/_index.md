---
title: HorizontalPageBreak
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents a horizontal page break.
type: docs
url: /sv/javascript-cpp/horizontalpagebreak/
---

## HorizontalPageBreak class

Encapsulates the object that represents a horizontal page break.

```javascript
class HorizontalPageBreak;
```


### Example
```javascript
const { Workbook } = AsposeCells;

//Instansiering av ett Workbook-objekt
var workbook = new Workbook();

//Hämtar referensen till det nyss tillagda kalkylbladet genom att skicka dess bladindex
var worksheet = workbook.worksheets.get(0);

//Lägg till en sidbrytning i cell Y30
var Index = worksheet.horizontalPageBreaks.add("Y30");

//hämta den nyss tillagda horisontella sidbrytningen
var hPageBreak = worksheet.horizontalPageBreaks.get(Index);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [startColumn](#startColumn--)| number | Readonly. Gets the start column index of this horizontal page break. |
| [endColumn](#endColumn--)| number | Readonly. Gets the end column index of this horizontal page break. |
| [row](#row--)| number | Readonly. Gets the zero based row index. |


### startColumn {#startColumn--}

Readonly. Gets the start column index of this horizontal page break.

```javascript
startColumn : number;
```


### endColumn {#endColumn--}

Readonly. Gets the end column index of this horizontal page break.

```javascript
endColumn : number;
```


### row {#row--}

Readonly. Gets the zero based row index.

```javascript
row : number;
```



