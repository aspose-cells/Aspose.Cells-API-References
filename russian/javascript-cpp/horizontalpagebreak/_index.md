---
title: HorizontalPageBreak
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents a horizontal page break.
type: docs
url: /ru/javascript-cpp/horizontalpagebreak/
---

## HorizontalPageBreak class

Encapsulates the object that represents a horizontal page break.

```javascript
class HorizontalPageBreak;
```


### Example
```javascript
const { Workbook } = AsposeCells;

//Создание объекта Workbook
var workbook = new Workbook();

//Получение ссылки на только что добавленный лист, передавая его индекс листа
var worksheet = workbook.worksheets.get(0);

//Добавьте разрыв страницы в ячейке Y30
var Index = worksheet.horizontalPageBreaks.add("Y30");

//получите недавно добавленный горизонтальный разрыв страницы
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



