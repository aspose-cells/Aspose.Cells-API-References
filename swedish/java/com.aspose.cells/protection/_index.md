---
title: "Skydd"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Representerar de olika typerna av skyddsalternativ som finns tillgängliga för ett kalkylblad.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Kopiera skyddsinformation. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Anger om raderingen av kolumner är tillåten på ett skyddat kalkylblad. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Anger om raderingen av rader är tillåten på ett skyddat kalkylblad. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Anger om användaren får redigera innehållet i låsta celler på ett skyddat kalkylblad. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Anger om användaren får manipulera ritobjekt på ett skyddat kalkylblad. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Anger om användaren får redigera scenarier på ett skyddat kalkylblad. |
| [getAllowFiltering()](#getAllowFiltering--) | Anger om användaren får använda ett AutoFilter som skapades innan bladet skyddades. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Anger om formatering av celler är tillåten på ett skyddat kalkylblad. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Anger om formatering av kolumner är tillåten på ett skyddat kalkylblad |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Anger om formatering av rader är tillåten på ett skyddat kalkylblad |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Anger om infogning av kolumner är tillåten på ett skyddat kalkylblad |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Anger om infogning av hyperlänkar är tillåten på ett skyddat kalkylblad |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Anger om infogning av rader är tillåten på ett skyddat kalkylblad |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Anger om användaren får markera låsta celler på ett skyddat kalkylblad. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Anger om användaren får markera olåsta celler på ett skyddat kalkylblad. |
| [getAllowSorting()](#getAllowSorting--) | Anger om sorteringsalternativet är tillåtet på ett skyddat kalkylblad. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Anger om användaren får manipulera pivottabeller på ett skyddat kalkylblad. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Anger lösenordet för att skydda kalkylbladet. |
| [getPasswordHash()](#getPasswordHash--) | Hämtar hashvärdet för det aktuella lösenordet. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Anger om kalkylbladet är skyddat med lösenord. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Anger om raderingen av kolumner är tillåten på ett skyddat kalkylblad. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Anger om raderingen av rader är tillåten på ett skyddat kalkylblad. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Anger om användaren får redigera innehållet i låsta celler på ett skyddat kalkylblad. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Anger om användaren får manipulera ritobjekt på ett skyddat kalkylblad. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Anger om användaren får redigera scenarier på ett skyddat kalkylblad. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Anger om användaren får använda ett AutoFilter som skapades innan bladet skyddades. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Anger om formatering av celler är tillåten på ett skyddat kalkylblad. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Anger om formatering av kolumner är tillåten på ett skyddat kalkylblad |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Anger om formatering av rader är tillåten på ett skyddat kalkylblad |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Anger om infogning av kolumner är tillåten på ett skyddat kalkylblad |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Anger om infogning av hyperlänkar är tillåten på ett skyddat kalkylblad |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Anger om infogning av rader är tillåten på ett skyddat kalkylblad |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Anger om användaren får markera låsta celler på ett skyddat kalkylblad. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Anger om användaren får markera olåsta celler på ett skyddat kalkylblad. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Anger om sorteringsalternativet är tillåtet på ett skyddat kalkylblad. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Anger om användaren får manipulera pivottabeller på ett skyddat kalkylblad. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Anger lösenordet för att skydda kalkylbladet. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Verifierar lösenord. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Kopiera skyddsinformation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Anger om raderingen av kolumner är tillåten på ett skyddat kalkylblad.

**Remarks**

Kolumnerna som innehåller cellerna som ska raderas måste vara olåsta när bladet är skyddat, och alternativet "Markera olåsta celler" måste vara aktiverat.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Anger om raderingen av rader är tillåten på ett skyddat kalkylblad.

**Remarks**

Raderna som innehåller cellerna som ska tas bort måste låsas upp när bladet är skyddat, och alternativet "Select unlocked cells" måste vara aktiverat.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Anger om användaren får redigera innehållet i låsta celler på ett skyddat kalkylblad.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Anger om användaren får manipulera ritobjekt på ett skyddat kalkylblad.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Anger om användaren får redigera scenarier på ett skyddat kalkylblad.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Anger om användaren får använda ett AutoFilter som skapades innan bladet skyddades.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Anger om formatering av celler är tillåten på ett skyddat kalkylblad.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Anger om formatering av kolumner är tillåten på ett skyddat kalkylblad

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Anger om formatering av rader är tillåten på ett skyddat kalkylblad

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Anger om infogning av kolumner är tillåten på ett skyddat kalkylblad

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Anger om infogning av hyperlänkar är tillåten på ett skyddat kalkylblad

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Anger om infogning av rader är tillåten på ett skyddat kalkylblad

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Anger om användaren får markera låsta celler på ett skyddat kalkylblad.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Anger om användaren får markera olåsta celler på ett skyddat kalkylblad.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Anger om sorteringsalternativet är tillåtet på ett skyddat kalkylblad.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Anger om användaren får manipulera pivottabeller på ett skyddat kalkylblad.

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


Anger lösenordet för att skydda kalkylbladet.

**Remarks**

Om lösenordet är satt till null eller en tom sträng kan du avskydda arbetsbladet eller arbetsboken utan att använda ett lösenord. Annars måste du ange lösenordet för att avskydda arbetsbladet eller arbetsboken.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Hämtar hashvärdet för det aktuella lösenordet.

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


Anger om kalkylbladet är skyddat med lösenord.

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


Anger om raderingen av kolumner är tillåten på ett skyddat kalkylblad.

**Remarks**

Kolumnerna som innehåller cellerna som ska raderas måste vara olåsta när bladet är skyddat, och alternativet "Markera olåsta celler" måste vara aktiverat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


Anger om raderingen av rader är tillåten på ett skyddat kalkylblad.

**Remarks**

Raderna som innehåller cellerna som ska tas bort måste låsas upp när bladet är skyddat, och alternativet "Select unlocked cells" måste vara aktiverat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


Anger om användaren får redigera innehållet i låsta celler på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


Anger om användaren får manipulera ritobjekt på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


Anger om användaren får redigera scenarier på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


Anger om användaren får använda ett AutoFilter som skapades innan bladet skyddades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


Anger om formatering av celler är tillåten på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


Anger om formatering av kolumner är tillåten på ett skyddat kalkylblad

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


Anger om formatering av rader är tillåten på ett skyddat kalkylblad

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


Anger om infogning av kolumner är tillåten på ett skyddat kalkylblad

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


Anger om infogning av hyperlänkar är tillåten på ett skyddat kalkylblad

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


Anger om infogning av rader är tillåten på ett skyddat kalkylblad

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


Anger om användaren får markera låsta celler på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


Anger om användaren får markera olåsta celler på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


Anger om sorteringsalternativet är tillåtet på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


Anger om användaren får manipulera pivottabeller på ett skyddat kalkylblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Anger lösenordet för att skydda kalkylbladet.

**Remarks**

Om lösenordet är satt till null eller en tom sträng kan du avskydda arbetsbladet eller arbetsboken utan att använda ett lösenord. Annars måste du ange lösenordet för att avskydda arbetsbladet eller arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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


Verifierar lösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | Lösenordet. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

