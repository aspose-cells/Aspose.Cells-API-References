---
title: "CellsDataTableFactory Class"
linktitle: "CellsDataTableFactory"
articleTitle: "CellsDataTableFactory"
second_title: "Aspose.Cells for Python via Java"
description: "Utility to build ICellsDataTable from custom objects for user's convenience."
type: docs
weight: 640
url: /python-java/asposecells.api/cellsdatatablefactory/
---

## CellsDataTableFactory class

Utility to build ICellsDataTable from custom objects for user's convenience.

## Methods

| Name | Description |
| --- | --- |
| [getInstance](#getinstance) | Creates ICellsDataTable from given sequence of int values. |

### getInstance(vals, columnNames) (1 of 12) {#getinstance}

Creates ICellsDataTable from given sequence of int values.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | Number Array | int values to build table |
| columnNames | String[] | Column names of the table. Its length can only be either 1(build table by the int values vertically) or length of the int values(build table by the int values horizontally) |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals, vertial) (2 of 12) {#getinstance-1}

Creates ICellsDataTable from given sequence of int values.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | Number Array | int values to build table |
| vertial | boolean | whether build table by the int values vertiacally(true) or horizontally(false) |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals, columnNames) (3 of 12) {#getinstance-2}

Creates ICellsDataTable from given sequence of double values.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | Number Array | double values to build table |
| columnNames | String[] | Column names of the table. Its length can only be either 1(build table by the double values vertically) or length of the double values(build table by the double values horizontally) |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals, vertial) (4 of 12) {#getinstance-3}

Creates ICellsDataTable from given sequence of double values.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | Number Array | double values to build table |
| vertial | boolean | whether build table by the double values vertiacally(true) or horizontally(false) |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals, columnNames) (5 of 12) {#getinstance-4}

Creates ICellsDataTable from given sequence of objects.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | Object[] | objects to build table |
| columnNames | String[] | Column names of the table. Its length can only be either 1(build table by the objects vertically) or length of the objects(build table by the objects horizontally) |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals, hasHeader, columnNames) (6 of 12) {#getinstance-5}

---

### getInstance(vals, vertial) (7 of 12) {#getinstance-6}

Creates ICellsDataTable from given sequence of objects.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | Object[] | objects to build table |
| vertial | boolean | whether build table by the objects vertiacally(true) or horizontally(false) |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals) (8 of 12) {#getinstance-7}

Creates ICellsDataTable from given 2D array.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | int[][] | int values to build table |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals) (9 of 12) {#getinstance-8}

Creates ICellsDataTable from given 2D array.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | double[][] | double values to build table |

**Returns:** Instance of ICellsDataTable

---

### getInstance(vals) (10 of 12) {#getinstance-9}

Creates ICellsDataTable from given 2D array.

| Parameter | Type | Description |
| --- | --- | --- |
| vals | Object[][] | objects to build table |

**Returns:** Instance of ICellsDataTable

---

### getInstance(collection) (11 of 12) {#getinstance-10}

Creates ICellsDataTable from given collection.

| Parameter | Type | Description |
| --- | --- | --- |
| collection | Collection | the collection to build table |

**Returns:** Instance of ICellsDataTable

---

### getInstance(collection, hasHeader) (12 of 12) {#getinstance-11}
