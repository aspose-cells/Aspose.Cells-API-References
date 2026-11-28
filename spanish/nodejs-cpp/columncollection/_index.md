---
title: ColumnCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Collection of the Column..column objects that represent the individual columnsettings in a worksheet. The Column object only represents the settings such as column width styles .etc. for the whole column has nothing to do with the fact that there are nonempty cellsdata or not in corresponding column. And the Count of this collection only represents the count Column objects that have been instantiated in this collection has nothing to do with the fact that there are nonempty cellsdata or not in the worksheet.
type: docs
url: /es/nodejs-cpp/columncollection/
---

## ColumnCollection class

Collection of the [Column](../column/) objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

```javascript
class ColumnCollection implements Iterable<Column>;
```


### Example
```javascript
const { Workbook, Color, BackgroundType, StyleFlag } = require("aspose.cells.node");

//Instanciando un objeto Workbook
var workbook = new Workbook();
//Obtener la referencia de la primera hoja de cálculo
var worksheet = workbook.worksheets.get(0);
//Agregar nuevo estilo al libro de trabajo
var style = workbook.createStyle();
//Estableciendo el color de fondo a azul
style.foregroundColor = Color.Blue;
//estableciendo patrón de fondo
style.pattern = BackgroundType.Solid;
//Nuevo indicador de estilo
var styleFlag = new StyleFlag();
//Establecer todos los estilos
styleFlag.all = true;

//Cambiar el ancho predeterminado de las primeras diez columnas
for (var i = 0; i < 10; i++) {
    worksheet.cells.columns.get(i).width = 20;
}

//Obtener la columna con formato no predeterminado
var columns = worksheet.cells.columns;
var count = columns.count;
for (var i = 0; i < count; i++) {
    var column = columns.getColumnByIndex(i);
    //Aplicar estilo a las primeras diez columnas
    column.applyStyle(style, styleFlag);
}

//Guardando el archivo Excel
workbook.save("output/ColumnCollection.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Column](../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before. |
| [getColumnByIndex(number)](#getColumnByIndex-number-)| Gets the [Column](../column/) object by the position in the list. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<Column\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### get(number) {#get-number-}

Gets a [Column](../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.

```javascript
get(columnIndex: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number |  |

**Returns**

[Column](../column/)

### getColumnByIndex(number) {#getColumnByIndex-number-}

Gets the [Column](../column/) object by the position in the list.

```javascript
getColumnByIndex(index: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position in the list. |

**Returns**

Returns the column object.

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



