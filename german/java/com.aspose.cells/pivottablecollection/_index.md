---
title: "PivotTableCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Sammlung aller PivotTable-Objekte im angegebenen Arbeitsblatt dar."
type: docs
url: /de/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Stellt die Sammlung aller PivotTable-Objekte im angegebenen Arbeitsblatt dar.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu. |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts mit Standardoptionen hinzu. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | Fügt eine neue PivotTable an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts hinzu. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu. |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts mit Standardoptionen hinzu. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts mit Standardoptionen hinzu. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Fügt eine neue PivotTable hinzu. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Fügt ein neues PivotTable‑Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Fügt ein neues PivotTable‑Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden. |
| [clear()](#clear--) | Löscht alle PivotTables. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [dispose()](#dispose--) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft den PivotTable‑Bericht nach Index ab. |
| [get(int row, int column)](#get-int-int-) | Ruft die im Zellbereich befindliche [PivotTable](../../com.aspose.cells/pivottable) ab. |
| [get(String name)](#get-java.lang.String-) | Ruft den PivotTable-Bericht anhand des Namens der PivotTable ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Löscht die angegebene PivotTable und löscht die PivotTable-Daten. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Löscht die angegebene PivotTable. |
| [removeAt(int index)](#removeAt-int-) | Löscht die PivotTable am angegebenen Index und löscht die PivotTable-Daten. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Löscht die PivotTable am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Die Quell-PivotTable. |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte PivotTable-Index.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Die Quell-PivotTable. |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte PivotTable-Index.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts mit Standardoptionen hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| Zeile | int | Der nullbasierte Zeilenindex der oberen linken Ecke des PivotTable-Ziels. |
| Spalte | int | Der nullbasierte Spaltenindex der oberen linken Ecke des PivotTable-Ziels. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


Fügt eine neue PivotTable an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| Zeile | int | Der nullbasierte Zeilenindex der oberen linken Ecke des PivotTable-Ziels. |
| Spalte | int | Der nullbasierte Spaltenindex der oberen linken Ecke des PivotTable-Ziels. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Optionen zur Erstellung von PivotTables. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu.

**Remarks**

HINWEIS: Diese Methode ist veraltet. Sie entspricht dem Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der Index in dieser PivotTable-Liste.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu.

**Remarks**

HINWEIS: Diese Methode ist veraltet. Sie entspricht dem Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits nutzt. Wenn die Eigenschaft true ist, spart dies Speicher. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu.

**Remarks**

HINWEIS: Diese Methode ist veraltet. Sie entspricht dem Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach Oktober 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits nutzt. Wenn die Eigenschaft true ist, spart dies Speicher. |
| isXlsClassic | boolean | Gibt an, ob eine klassische PivotTable von Excel 97-2003 hinzugefügt wird. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts mit Standardoptionen hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| cellName | java.lang.String | Der Name der Zelle in der oberen linken Ecke für das PivotTable-Ziel. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


Fügt eine neue moderne PivotTable (seit Excel 2007) an der angegebenen Zeilen‑ und Spaltenposition des Arbeitsblatts mit Standardoptionen hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| cellName | java.lang.String | Der Name der Zelle in der oberen linken Ecke für das PivotTable-Ziel. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Die Optionen zum Erstellen einer PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu.

**Remarks**

HINWEIS: Diese Methode ist veraltet. Sie entspricht dem Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Die Daten für den neuen PivotTable-Cache. |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der Index in dieser PivotTable-Liste.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Fügt eine neue PivotTable mit dem Legacy‑Layout und -Stil von Excel 97‑2003 hinzu.

**Remarks**

HINWEIS: Diese Methode ist veraltet. Sie entspricht dem Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach September 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Die Daten für den neuen PivotTable-Cache. |
| destCellName | java.lang.String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits nutzt. Wenn die Eigenschaft true ist, spart dies Speicher. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Fügt eine neue PivotTable hinzu.

**Remarks**

HINWEIS: Diese Methode ist veraltet. Sie entspricht dem Aufruf von PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) mit `NewPivotTableOptions.IsXlsClassic = true`. Bitte verwenden Sie stattdessen die Überladung PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Diese Methode wird 12 Monate nach Oktober 2026 entfernt. Wir entschuldigen uns für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String | Der Datenzellenbereich für die neue PivotTable. Beispiel: Sheet1!A1:C8 |
| Zelle | java.lang.String | Die Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |
| useSameSource | boolean | Gibt an, ob dieselbe Datenquelle verwendet wird, wenn eine andere vorhandene PivotTable diese Datenquelle bereits verwendet hat. Ist die Eigenschaft wahr, spart sie Speicher, wenn dieselbe Datenquelle in einem Pivot-Cache zusammengefasst wurde. |
| isXlsClassic | boolean | Gibt an, ob eine klassische PivotTable von Excel 97-2003 hinzugefügt wird. |

**Returns:**
int - Der neu hinzugefügte Cache-Index.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Fügt ein neues PivotTable‑Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String[] | Die mehreren Konsolidierungsbereiche, z. B. \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Gibt an, ob ein einzelnes Seitenfeld automatisch erstellt wird. Ist es wahr, wird der folgende Parameter pageFields ignoriert. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Die Pivot-Seitenfeld-Elemente. |
| Zeile | int | Zeilenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| Spalte | int | Spaltenindex der Zelle in der oberen linken Ecke des Zielbereichs des PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte PivotTable-Index.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Fügt ein neues PivotTable‑Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceData | java.lang.String[] | Die mehreren Konsolidierungsbereiche, z. B. \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Gibt an, ob ein einzelnes Seitenfeld automatisch erstellt wird. Ist es wahr, wird der folgende Parameter pageFields ignoriert. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Die Pivot-Seitenfeld-Elemente. |
| destCellName | java.lang.String | destCellName Der Name des neuen PivotTable-Berichts. |
| tableName | java.lang.String | Der Name des neuen PivotTable-Berichts. |

**Returns:**
int - Der neu hinzugefügte PivotTable-Index.
### clear() {#clear--}
```
public void clear()
```


Löscht alle PivotTables.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
### dispose() {#dispose--}
```
public void dispose()
```


Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public PivotTable get(int index)
```


Ruft den PivotTable‑Bericht nach Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Ruft die im Zellbereich befindliche [PivotTable](../../com.aspose.cells/pivottable) ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int |  |
| Spalte | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


Ruft den PivotTable-Bericht anhand des Namens der PivotTable ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Löscht die angegebene PivotTable und löscht die PivotTable-Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Löscht die angegebene PivotTable.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-Objekt |
| keepData | boolean | Gibt an, ob die PivotTable-Daten beibehalten werden sollen |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Löscht die PivotTable am angegebenen Index und löscht die PivotTable-Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Positionsindex in der PivotTable-Sammlung |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Löscht die PivotTable am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Positionsindex in der PivotTable-Sammlung |
| keepData | boolean | Gibt an, ob die PivotTable-Daten beibehalten werden sollen |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

