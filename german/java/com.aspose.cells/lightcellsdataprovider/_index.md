---
title: "LightCellsDataProvider"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Datenanbieter zum Speichern großer Tabellenkalkulationsdateien im Leichtgewichtsmodus dar."
type: docs
url: /de/java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

Stellt den Datenanbieter zum Speichern großer Tabellenkalkulationsdateien im Leichtgewichtsmodus dar.

**Remarks**

Beim Speichern einer Arbeitsmappe mit diesem Modus wird [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) bei jedem Speichern eines Arbeitsblatts in der Arbeitsmappe geprüft. Für ein Blatt, wenn [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) true zurückgibt, werden alle zu speichernden Daten und Eigenschaften für Zeilen/Zellen dieses Blatts von der Implementierung dieses Interfaces bereitgestellt. Zunächst wird [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) aufgerufen, um den nächsten Zeilenindex zu erhalten, der gespeichert werden soll. Wenn ein gültiger Zeilenindex zurückgegeben wird (der Zeilenindex muss für die zu speichernden Zeilen in aufsteigender Reihenfolge vorliegen), wird ein Row-Objekt, das diese Zeile repräsentiert, von [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-) für die Implementierung bereitgestellt, um dessen Eigenschaften zu setzen. Für eine Zeile wird zunächst [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--) geprüft. Wenn ein gültiger Spaltenindex zurückgegeben wird (der Spaltenindex muss für alle Zellen der aktuellen Zeile in aufsteigender Reihenfolge vorliegen), wird ein Cell-Objekt, das diese Zelle repräsentiert, von [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) für die Implementierung bereitgestellt, um dessen Daten und Eigenschaften zu setzen. Nach [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) wird die Zelle direkt in die resultierende Tabellenkalkulationsdatei gespeichert. Dann wird die nächste Zelle geprüft und verarbeitet.

Bitte beachten Sie, dass der Benutzer nur Werte und Eigenschaften für das aktuelle Row/Cell-Objekt aktualisieren sollte, das von der entsprechenden Methode bereitgestellt wird. Da die Zellen­daten in Streaming‑Manier in die resultierende Datei geschrieben werden, können die meisten anderen Objekte bereits in die resultierende Datei geschrieben sein oder es wurden globale Daten für sie gesammelt und geschrieben. Wenn der Benutzer also andere Objekte aktualisiert, während Zellen­daten gespeichert werden, können diese Vorgänge die gespeicherten Daten möglicherweise nicht beeinflussen. Noch schlimmer kann es dazu führen, dass inkonsistente Daten in die resultierende Datei gespeichert werden und die Datei schließlich beschädigt wird. Daher sollten Sie für alle anderen Objekte wie Formen, Spaltenbreiten und Stile, bedingte Formatierungen usw. in keinen Methoden dieser Implementierung operieren. Stattdessen verwalten und passen Sie sie bitte vor dem Aufruf der "Save"‑Methode des Workbook an den Endzustand an.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [isGatherString()](#isGatherString--) | Prüft, ob der aktuelle Zeichenkettenwert der Zelle in einen globalen Pool aufgenommen werden muss. |
| [nextCell()](#nextCell--) | Liefert die nächste zu speichernde Zelle. |
| [nextRow()](#nextRow--) | Liefert die nächste zu speichernde Zeile. |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | Beginnt mit dem Speichern der Daten einer Zelle. |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | Beginnt mit dem Speichern der Daten einer Zeile. |
| [startSheet(int sheetIndex)](#startSheet-int-) | Beginnt mit dem Speichern eines Arbeitsblatts. |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


Prüft, ob der aktuelle Zeichenkettenwert der Zelle in einen globalen Pool aufgenommen werden muss.

**Remarks**

Das Sammeln von Zeichenkettenwerten ist nur vorteilhaft, wenn es viele duplizierte Zeichenkettenwerte für die von dieser Implementierung bereitgestellten Zellen gibt. In diesem Fall spart das Sammeln von Zeichenketten viel Speicher und erzeugt eine kleinere Ergebnisdatei. Wenn es viele Zeichenkettenwerte für die von LightCellsDataProvider bereitgestellten Zellen gibt, aber nur wenige davon identisch sind, kostet das Sammeln von Zeichenketten mehr Speicher und Zeit und bietet keinen Vorteil für die Ergebnisdatei.

**Returns:**
boolean - true, wenn der Zeichenkettenwert in einen globalen Pool für die resultierende Datei aufgenommen werden muss.
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


Liefert die nächste zu speichernde Zelle.

**Remarks**

Wird zu Beginn des Speicherns einer Zelle aufgerufen.

**Returns:**
int - Spaltenindex der nächsten zu speichernden Zelle. -1 bedeutet, dass das Ende der aktuellen Zeilendaten erreicht wurde und keine weitere Zelle der aktuellen Zeile mehr gespeichert wird.
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


Liefert die nächste zu speichernde Zeile.

**Remarks**

Wird zu Beginn des Speicherns einer Zeile und ihrer Zellen­daten aufgerufen (vor [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-)).

**Returns:**
int - der nächste Zeilenindex, der gespeichert werden soll. -1 bedeutet, dass das Ende der aktuellen Blattdaten erreicht wurde und keine weitere Zeile des aktuellen Blatts mehr gespeichert wird.
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


Beginnt mit dem Speichern der Daten einer Zelle.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Cell-Objekt für die Implementierung zum Befüllen von Daten. Sein Spaltenindex ist der Rückgabewert des letzten Aufrufs von [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--). Wenn die Zelle im inneren Zellenmodell initialisiert wurde, wird das vorhandene Zellenobjekt verwendet. Andernfalls wird ein temporäres Cell-Objekt für die Implementierung zum Befüllen von Daten verwendet. |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


Beginnt mit dem Speichern der Daten einer Zeile.

**Remarks**

Wird zu Beginn des Speicherns einer Zeile und ihrer Zellen­daten aufgerufen. Wenn die aktuelle Zeile benutzerdefinierte Eigenschaften wie Höhe, Stil, … usw. hat, sollte die Implementierung diese Eigenschaften hier im übergebenen Row‑Objekt setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Row‑Objekt für die Implementierung zum Befüllen von Daten. Sein Zeilenindex ist der Rückgabewert des letzten Aufrufs von [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--). Wenn die Zeile im inneren Zellenmodell initialisiert wurde, wird das vorhandene Zeilenobjekt verwendet. Andernfalls wird ein temporäres Row‑Objekt für die Implementierung zum Befüllen von Daten verwendet. |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


Beginnt mit dem Speichern eines Arbeitsblatts.

**Remarks**

Wird zu Beginn des Speicherns eines Arbeitsblatts während des Speicherns einer Arbeitsmappe aufgerufen. Wenn der Provider später in der Methode startRow(Row) oder startCell(Cell) auf *`sheetIndex`* verweisen muss, also wenn der Vorgang wissen muss, welches Arbeitsblatt verarbeitet wird, sollte die Implementierung den Wert von *`sheetIndex`* hier behalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Index des zu speichernden aktuellen Blatts. |

**Returns:**
boolean - true, wenn dieser Provider Daten für das angegebene Blatt bereitstellt; false, wenn das angegebene Blatt sein normales Datenmodell (Cells) verwenden soll.
