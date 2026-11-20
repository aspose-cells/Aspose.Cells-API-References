---
title: "LightCellsDataHandler"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Zellen‑Daten‑Handler zum Lesen großer Tabellenkalkulationsdateien im Leichtgewichtsmodus dar."
type: docs
url: /de/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

Stellt den Zellen‑Daten‑Handler zum Lesen großer Tabellenkalkulationsdateien im Leichtgewichtsmodus dar.

**Remarks**

Beim Lesen einer Arbeitsmappe in diesem Modus wird [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) bei jedem Lesen eines Arbeitsblatts in der Arbeitsmappe geprüft. Für ein Blatt, wenn [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) true zurückgibt, werden alle Daten und Eigenschaften von Zeilen/Zellen dieses Blatts von der Implementierung dieses Interfaces geprüft und verarbeitet. Für jede Zeile wird [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) aufgerufen, um zu prüfen, ob sie verarbeitet werden muss. Wenn eine Zeile verarbeitet werden muss, werden zunächst die Eigenschaften dieser Zeile gelesen und der Benutzer kann über [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) auf ihre Eigenschaften zugreifen. Wenn die Zellen der Zeile ebenfalls verarbeitet werden müssen, sollte [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) true zurückgeben und dann wird [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) für jede vorhandene Zelle in dieser Zeile aufgerufen, um zu prüfen, ob eine Zelle verarbeitet werden muss. Wenn eine Zelle verarbeitet werden muss, wird [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) aufgerufen, um die Zelle durch die Implementierung dieses Interfaces zu verarbeiten.

Bitte beachten Sie, dass der Benutzer nur an den Werten und Eigenschaften des aktuellen Row/Cell-Objekts, das von der entsprechenden Methode bereitgestellt wird, arbeiten sollte. Da die Zellen­daten aus der Vorlagendatei in Streaming‑Manier gelesen werden, können die meisten anderen Objekte später nach dem Laden der Zellen­daten zurückgesetzt/aktualisiert werden. Wenn der Benutzer also in dieser Implementierung andere Objekte verwendet, können diese Vorgänge die im Workbook vorhandenen Objekte möglicherweise nicht beeinflussen. Noch schlimmer kann es zu inkonsistenten Daten im Workbook führen und später unerwartete Probleme oder Ausnahmen verursachen. Daher sollten Sie für alle anderen Objekte wie Formen, Spaltenbreite und Stile, bedingte Formatierungen usw. in keinen Methoden dieser Implementierung arbeiten. Stattdessen verwalten Sie sie bitte, nachdem das Workbook erstellt wurde.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | Beginnt mit der Verarbeitung einer Zelle. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | Beginnt mit der Verarbeitung einer Zeile. |
| [startCell(int columnIndex)](#startCell-int-) | Bereitet die Verarbeitung einer Zelle vor. |
| [startRow(int rowIndex)](#startRow-int-) | Bereitet die Verarbeitung einer Zeile vor. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Beginnt mit der Verarbeitung eines Arbeitsblatts. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


Beginnt mit der Verarbeitung einer Zelle.

**Remarks**

Wird aufgerufen, nachdem die Daten einer Zelle gelesen wurden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Zellenobjekt, das derzeit verarbeitet wird |

**Returns:**
boolean – gibt an, ob diese Zelle im Zellen‑Modell des aktuellen Blatts behalten werden muss. In der Regel sollte es false sein, damit alle Zellen nach der Verarbeitung nicht im Speicher gehalten werden und Speicher gespart wird. Für spezielle Zwecke, z. B. wenn der Benutzer später nach der vollständigen Verarbeitung des Workbooks auf einige Zellen zugreifen muss, kann diese Methode true zurückgeben, um diese besonderen Zellen im Cells‑Modell zu behalten und später über APIs wie Cells[row, column] darauf zuzugreifen. Das Behalten von Zellen­daten im Cells‑Modell erfordert jedoch mehr Speicher, und wenn alle Zellen behalten werden, wird das Lesen der Vorlagendatei im LightCells‑Modus dasselbe wie das normale Lesen.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


Beginnt mit der Verarbeitung einer Zeile.

**Remarks**

Wird aufgerufen, nachdem die Eigenschaften der Zeile wie Höhe, Stil, ...etc. gelesen wurden. Die Zellen dieser Zeile wurden jedoch noch nicht gelesen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Zeilenobjekt, das derzeit verarbeitet wird. |

**Returns:**
boolean – gibt an, ob die Zellen dieser Zeile verarbeitet werden müssen. false, um alle Zellen in dieser Zeile zu ignorieren.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


Bereitet die Verarbeitung einer Zelle vor.

**Remarks**

Wird aufgerufen, wenn eine vorhandene Zelle in der aktuellen Zeile erreicht wird. Die aktuelle Zeile ist die Zeile des letzten Aufrufs von [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex der zu verarbeitenden Zelle |

**Returns:**
boolean – gibt an, ob diese Zelle verarbeitet werden muss. false, um die Zelle zu ignorieren und die nächste zu prüfen, bis das Ende der Zellen­daten der aktuellen Zeile erreicht ist.
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


Bereitet die Verarbeitung einer Zeile vor.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | int | Index der nächsten zu verarbeitenden Zeile |

**Returns:**
boolean – gibt an, ob diese Zeile (Eigenschaften oder Zellen­daten) verarbeitet werden muss. false, um diese Zeile und ihre Zellen zu ignorieren und die nächste Zeile zu prüfen.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


Beginnt mit der Verarbeitung eines Arbeitsblatts.

**Remarks**

Wird aufgerufen, bevor die Zellen­daten eines Arbeitsblatts gelesen werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Das Arbeitsblatt, dessen Zellen­daten gelesen werden sollen. |

**Returns:**
boolean – gibt an, ob die Zellen­daten dieses Blatts verarbeitet werden müssen. false, um dieses Blatt zu ignorieren.
