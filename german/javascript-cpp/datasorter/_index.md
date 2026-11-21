---
title: DataSorter
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Summary description for DataSorter.
type: docs
url: /de/javascript-cpp/datasorter/
---

## DataSorter class

Summary description for DataSorter.

```javascript
class DataSorter;
```


### Example
```javascript
const { Workbook, CellArea, SortOrder, SaveFormat } = AsposeCells;

//Ein neues Workbook-Objekt instanziieren.
var workbook = new Workbook(data);
//Das Workbook-Datasorter-Objekt abrufen.
var sorter = workbook.dataSorter;
//Den ersten Sortiermodus für das Datasorter-Objekt festlegen.
sorter.order1 = SortOrder.Descending;
//Den ersten Schlüssel definieren.
sorter.key1 = 0;
//Einen Zellenbereich (Range) erstellen.
var ca = new CellArea();
//Startzeilenindex angeben.
ca.startRow = 0;
//Startspaltenindex angeben.
ca.startColumn = 0;
//Letzten Zeilenindex angeben.
ca.endRow = 12;
//Letzten Spaltenindex angeben.
ca.endColumn = 1;
//Daten im angegebenen Datenbereich (A1:B14) sortieren
sorter.sort(workbook.worksheets.get(0).cells, ca);
//Speichern Sie die Excel-Datei.
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [keys](#keys--)| DataSorterKeyCollection | Readonly. Gets the key list of data sorter. |
| [hasHeaders](#hasHeaders--)| boolean | Represents whether the range has headers. |
| [key1](#key1--)| number | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order1](#order1--)| SortOrder | Represents sort order of the first key. |
| [key2](#key2--)| number | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order2](#order2--)| SortOrder | Represents sort order of the second key. |
| [key3](#key3--)| number | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order3](#order3--)| SortOrder | Represents sort order of the third key. |
| [sortLeftToRight](#sortLeftToRight--)| boolean | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [caseSensitive](#caseSensitive--)| boolean | Gets and sets whether case sensitive when comparing string. |
| [sortAsNumber](#sortAsNumber--)| boolean | Indicates whether sorting anything that looks like a number. |

## Methods

| Method | Description |
| --- | --- |
| [clear()](#clear--)| Clear all settings. |
| [addKey(number, SortOrder)](#addKey-number-sortorder-)| Adds sorted column index and sort order. |
| [addKey(number, SortOrder, string)](#addKey-number-sortorder-string-)| Adds sorted column index and sort order with custom sort list. |
| [addKey(number, SortOnType, SortOrder, VObject)](#addKey-number-sortontype-sortorder-vobject-)| Adds sorted column index and sort order with custom sort list. |
| [addKey(number, SortOrder, string[])](#addKey-number-sortorder-stringarray-)| Adds sorted column index and sort order with custom sort list. |
| [addColorKey(number, SortOnType, SortOrder, Color)](#addColorKey-number-sortontype-sortorder-color-)| Adds color sort key. |
| [sort(Cells, number, number, number, number)](#sort-cells-number-number-number-number-)| Sorts the data of the area. |
| [sort(Cells, CellArea)](#sort-cells-cellarea-)| Sort the data of the area. |
| [sort()](#sort--)| Sort the data in the range. |


### keys {#keys--}

Readonly. Gets the key list of data sorter.

```javascript
keys : DataSorterKeyCollection;
```


### hasHeaders {#hasHeaders--}

Represents whether the range has headers.

```javascript
hasHeaders : boolean;
```


### key1 {#key1--}

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
key1 : number;
```


### order1 {#order1--}

Represents sort order of the first key.

```javascript
order1 : SortOrder;
```


### key2 {#key2--}

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
key2 : number;
```


### order2 {#order2--}

Represents sort order of the second key.

```javascript
order2 : SortOrder;
```


### key3 {#key3--}

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
key3 : number;
```


### order3 {#order3--}

Represents sort order of the third key.

```javascript
order3 : SortOrder;
```


### sortLeftToRight {#sortLeftToRight--}

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

```javascript
sortLeftToRight : boolean;
```


### caseSensitive {#caseSensitive--}

Gets and sets whether case sensitive when comparing string.

```javascript
caseSensitive : boolean;
```


### sortAsNumber {#sortAsNumber--}

Indicates whether sorting anything that looks like a number.

```javascript
sortAsNumber : boolean;
```


### clear() {#clear--}

Clear all settings.

```javascript
clear() : void;
```


### addKey(number, SortOrder) {#addKey-number-sortorder-}

Adds sorted column index and sort order.

```javascript
addKey(key: number, order: SortOrder) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order |

### addKey(number, SortOrder, string) {#addKey-number-sortorder-string-}

Adds sorted column index and sort order with custom sort list.

```javascript
addKey(key: number, order: SortOrder, customList: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | string | The custom sort list. |

### addKey(number, SortOnType, SortOrder, VObject) {#addKey-number-sortontype-sortorder-vobject-}

Adds sorted column index and sort order with custom sort list.

```javascript
addKey(key: number, type: SortOnType, order: SortOrder, customList: VObject) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | [SortOnType](../sortontype/) | The sorted value type. |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | VObject | The custom sort list. |

**Remarks**

If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.

### addKey(number, SortOrder, string[]) {#addKey-number-sortorder-stringarray-}

Adds sorted column index and sort order with custom sort list.

```javascript
addKey(key: number, order: SortOrder, customList: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | string[] | The custom sort list. |

### addColorKey(number, SortOnType, SortOrder, Color) {#addColorKey-number-sortontype-sortorder-color-}

Adds color sort key.

```javascript
addColorKey(key: number, type: SortOnType, order: SortOrder, color: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | [SortOnType](../sortontype/) | The sorted color value type. |
| order | [SortOrder](../sortorder/) | The sort order. |
| color | [Color](../color/) | The custom sort color. |

### sort(Cells, number, number, number, number) {#sort-cells-number-number-number-number-}

Sorts the data of the area.

```javascript
sort(cells: Cells, startRow: number, startColumn: number, endRow: number, endColumn: number) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../cells/) | The cells contains the data area. |
| startRow | number | The start row of the area. |
| startColumn | number | The start column of the area. |
| endRow | number | The end row of the area. |
| endColumn | number | The end column of the area. |

**Returns**

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### sort(Cells, CellArea) {#sort-cells-cellarea-}

Sort the data of the area.

```javascript
sort(cells: Cells, area: CellArea) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../cells/) | The cells contains the data area. |
| area | [CellArea](../cellarea/) | The area needed to sort |

**Returns**

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### sort() {#sort--}

Sort the data in the range.

```javascript
sort() : number[];
```


**Returns**

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.


