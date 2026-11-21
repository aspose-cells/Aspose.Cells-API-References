---
title: HorizontalPageBreak
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents a horizontal page break.
type: docs
url: /de/javascript-cpp/horizontalpagebreak/
---

## HorizontalPageBreak class

Encapsulates the object that represents a horizontal page break.

```javascript
class HorizontalPageBreak;
```


### Example
```javascript
const { Workbook } = AsposeCells;

//Instanziieren eines Workbook-Objekts
var workbook = new Workbook();

//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
var worksheet = workbook.worksheets.get(0);

//Füge einen Seitenumbruch bei Zelle Y30 hinzu
var Index = worksheet.horizontalPageBreaks.add("Y30");

//Hole den neu hinzugefügten horizontalen Seitenumbruch
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



