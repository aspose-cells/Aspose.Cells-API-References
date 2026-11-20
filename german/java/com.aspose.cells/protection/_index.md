---
title: "Schutz"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind."
type: docs
url: /de/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Stellt die verschiedenen Arten von Schutzoptionen dar, die für ein Arbeitsblatt verfügbar sind.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Kopiere Schutzinformationen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Gibt an, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Gibt an, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Gibt an, ob der Benutzer den Inhalt gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Gibt an, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Gibt an, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf. |
| [getAllowFiltering()](#getAllowFiltering--) | Gibt an, ob der Benutzer einen AutoFilter, der vor dem Schutz des Blatts erstellt wurde, verwenden darf. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Gibt an, ob die Formatierung von Zellen in einem geschützten Arbeitsblatt erlaubt ist. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Gibt an, ob die Formatierung von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Gibt an, ob die Formatierung von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Gibt an, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Gibt an, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Gibt an, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Gibt an, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Gibt an, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [getAllowSorting()](#getAllowSorting--) | Gibt an, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Gibt an, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Gibt das Passwort zum Schutz des Arbeitsblatts an. |
| [getPasswordHash()](#getPasswordHash--) | Ermittelt den Hash des aktuellen Passworts. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Gibt an, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Gibt an, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Gibt an, ob der Benutzer den Inhalt gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Gibt an, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Gibt an, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Gibt an, ob der Benutzer einen AutoFilter, der vor dem Schutz des Blatts erstellt wurde, verwenden darf. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Gibt an, ob die Formatierung von Zellen in einem geschützten Arbeitsblatt erlaubt ist. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Gibt an, ob die Formatierung von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Gibt an, ob die Formatierung von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Gibt an, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Gibt an, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Gibt an, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Gibt an, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Gibt an, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Gibt an, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Gibt an, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Gibt das Passwort zum Schutz des Arbeitsblatts an. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Überprüft das Passwort. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Kopiere Schutzinformationen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Gibt an, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist.

**Remarks**

Die Spalten, die die zu löschenden Zellen enthalten, müssen entsperrt sein, wenn das Blatt geschützt ist, und die Option "Entsperrte Zellen auswählen" muss aktiviert sein.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Gibt an, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist.

**Remarks**

Die Zeilen, die die zu löschenden Zellen enthalten, müssen entsperrt sein, wenn das Blatt geschützt ist, und die Option "Entsperrte Zellen auswählen" muss aktiviert sein.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Gibt an, ob der Benutzer den Inhalt gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Gibt an, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Gibt an, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Gibt an, ob der Benutzer einen AutoFilter, der vor dem Schutz des Blatts erstellt wurde, verwenden darf.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Gibt an, ob die Formatierung von Zellen in einem geschützten Arbeitsblatt erlaubt ist.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Gibt an, ob die Formatierung von Spalten in einem geschützten Arbeitsblatt erlaubt ist

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Gibt an, ob die Formatierung von Zeilen in einem geschützten Arbeitsblatt erlaubt ist

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Gibt an, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Gibt an, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Gibt an, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Gibt an, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Gibt an, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Gibt an, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Gibt an, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


Gibt das Passwort zum Schutz des Arbeitsblatts an.

**Remarks**

Wenn das Passwort auf null oder einen leeren String gesetzt ist, können Sie das Arbeitsblatt oder die Arbeitsmappe ohne Passwortschutz aufheben. Andernfalls müssen Sie das Passwort angeben, um das Arbeitsblatt oder die Arbeitsmappe zu entsperren.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Ermittelt den Hash des aktuellen Passworts.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Gibt an, ob das Arbeitsblatt mit einem Passwort geschützt ist.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


Gibt an, ob das Löschen von Spalten in einem geschützten Arbeitsblatt erlaubt ist.

**Remarks**

Die Spalten, die die zu löschenden Zellen enthalten, müssen entsperrt sein, wenn das Blatt geschützt ist, und die Option "Entsperrte Zellen auswählen" muss aktiviert sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


Gibt an, ob das Löschen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist.

**Remarks**

Die Zeilen, die die zu löschenden Zellen enthalten, müssen entsperrt sein, wenn das Blatt geschützt ist, und die Option "Entsperrte Zellen auswählen" muss aktiviert sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


Gibt an, ob der Benutzer den Inhalt gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


Gibt an, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


Gibt an, ob der Benutzer Szenarien in einem geschützten Arbeitsblatt bearbeiten darf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


Gibt an, ob der Benutzer einen AutoFilter, der vor dem Schutz des Blatts erstellt wurde, verwenden darf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


Gibt an, ob die Formatierung von Zellen in einem geschützten Arbeitsblatt erlaubt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


Gibt an, ob die Formatierung von Spalten in einem geschützten Arbeitsblatt erlaubt ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


Gibt an, ob die Formatierung von Zeilen in einem geschützten Arbeitsblatt erlaubt ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


Gibt an, ob das Einfügen von Spalten in einem geschützten Arbeitsblatt erlaubt ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


Gibt an, ob das Einfügen von Hyperlinks in einem geschützten Arbeitsblatt erlaubt ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


Gibt an, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


Gibt an, ob der Benutzer gesperrte Zellen in einem geschützten Arbeitsblatt auswählen darf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


Gibt an, ob der Benutzer entsperrte Zellen in einem geschützten Arbeitsblatt auswählen darf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


Gibt an, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


Gibt an, ob der Benutzer Pivot-Tabellen in einem geschützten Arbeitsblatt manipulieren darf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Gibt das Passwort zum Schutz des Arbeitsblatts an.

**Remarks**

Wenn das Passwort auf null oder einen leeren String gesetzt ist, können Sie das Arbeitsblatt oder die Arbeitsmappe ohne Passwortschutz aufheben. Andernfalls müssen Sie das Passwort angeben, um das Arbeitsblatt oder die Arbeitsmappe zu entsperren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


Überprüft das Passwort.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | java.lang.String | Das Passwort. |

**Returns:**
boolean -
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

