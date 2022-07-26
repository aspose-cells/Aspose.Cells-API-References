---
title: Add
second_title: Aspose.Cells für .NET-API-Referenz
description: Fügt einer PivotCaches-Sammlung einen neuen PivotTable-Cache hinzu.
type: docs
weight: 20
url: /de/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_4}

Fügt einer PivotCaches-Sammlung einen neuen PivotTable-Cache hinzu.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Die Daten für den neuen PivotTable-Cache. |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_5}

Fügt einer PivotCaches-Sammlung einen neuen PivotTable-Cache hinzu.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Die Daten für den neuen PivotTable-Cache. |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | Boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene Pivot-Tabelle diese Datenquelle verwendet hat. Wenn die Eigenschaft wahr ist, wird Speicher gespart. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

Fügt einer PivotCaches-Sammlung einen neuen PivotTable-Cache hinzu.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Datenzellenbereich für die neue PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

Fügt einer PivotCaches-Sammlung einen neuen PivotTable-Cache hinzu.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String | Der Datenzellenbereich für die neue PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | Boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene Pivot-Tabelle diese Datenquelle verwendet hat. Wenn die Eigenschaft wahr ist, wird Speicher gespart. |

### Rückgabewert

Der neu hinzugefügte Cache-Index.

### Siehe auch

* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

Fügt der Sammlung ein neues PivotTable-Objekt aus einer anderen PivotTable hinzu.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | PivotTable | Die Quell-PivotTable. |
| destCellName | String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte PivotTable-Index.

### Siehe auch

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

Fügt der Sammlung ein neues PivotTable-Objekt aus einer anderen PivotTable hinzu.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | PivotTable | Die Quell-PivotTable. |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte PivotTable-Index.

### Siehe auch

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_7}

Fügt der Sammlung ein neues PivotTable-Objekt mit mehreren Konsolidierungsbereichen als Datenquelle hinzu.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String[] | Die mehreren Konsolidierungsbereiche, z. B. {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Ob ein einzelnes Seitenfeld automatisch erstellt wird. Wenn wahr, wird der folgende Parameter pageFields ignoriert. |
| pageFields | PivotPageFields | Die Feldelemente der Pivot-Seite. |
| destCellName | String | destCellName Der Name des neuen PivotTable-Berichts. |
| tableName | String | der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte PivotTable-Index.

### Siehe auch

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_6}

Fügt der Sammlung ein neues PivotTable-Objekt mit mehreren Konsolidierungsbereichen als Datenquelle hinzu.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | String[] | Die mehreren Konsolidierungsbereiche, z. B. {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Ob ein einzelnes Seitenfeld automatisch erstellt wird. Wenn wahr, wird der folgende Parameter pageFields ignoriert |
| pageFields | PivotPageFields | Die Feldelemente der Pivot-Seite. |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | String | Der Name des neuen PivotTable-Berichts. |

### Rückgabewert

Der neu hinzugefügte PivotTable-Index.

### Siehe auch

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* namensraum [Aspose.Cells.Pivot](../../pivottablecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
