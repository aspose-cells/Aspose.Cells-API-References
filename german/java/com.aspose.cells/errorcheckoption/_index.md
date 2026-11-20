---
title: "ErrorCheckOption"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Fehlerprüfungs‑Einstellung, die auf bestimmte Bereiche angewendet wird."
type: docs
url: /de/java/com.aspose.cells/errorcheckoption/
---

**Inheritance:**
java.lang.Object
```
public class ErrorCheckOption
```

Fehlerprüfungs‑Einstellung, die auf bestimmte Bereiche angewendet wird.

**Example**

```
           Workbook workbook = new Workbook();
           ErrorCheckOptionCollection opts = workbook.getWorksheets().get(0).getErrorCheckOptions();
           int optionIdx = opts.add();
           ErrorCheckOption opt = opts.get(optionIdx);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_FORMULA, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_RANGE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_DATE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_NUMBER, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.VALIDATION, false);
           opt.addRange(CellArea.createCellArea("A1", "B10"));
           workbook.save("Book1.xlsx");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addRange(CellArea ca)](#addRange-com.aspose.cells.CellArea-) | Fügt einen von dieser Einstellung beeinflussten Bereich hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCountOfRange()](#getCountOfRange--) | Ermittelt die Anzahl der von dieser Einstellung beeinflussten Bereiche. |
| [getRange(int index)](#getRange-int-) | Ermittelt den von dieser Einstellung beeinflussten Bereich anhand des angegebenen Index. |
| [hashCode()](#hashCode--) |  |
| [isErrorCheck(int errorCheckType)](#isErrorCheck-int-) | Prüft, ob der angegebene Fehlertyp überprüft wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeRange(int index)](#removeRange-int-) | Entfernt einen Bereich anhand des angegebenen Index. |
| [setErrorCheck(int errorCheckType, boolean isCheck)](#setErrorCheck-int-boolean-) | Legt fest, ob der angegebene Fehlertyp überprüft wird. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(CellArea ca) {#addRange-com.aspose.cells.CellArea-}
```
public int addRange(CellArea ca)
```


Fügt einen von dieser Einstellung beeinflussten Bereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | der hinzuzufügende Bereich. |

**Returns:**
int - der Index des hinzugefügten Bereichs in der Bereichsliste dieser Einstellung.
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCountOfRange() {#getCountOfRange--}
```
public int getCountOfRange()
```


Ermittelt die Anzahl der von dieser Einstellung beeinflussten Bereiche.

**Returns:**
int - die Anzahl der von dieser Einstellung beeinflussten Bereiche.
### getRange(int index) {#getRange-int-}
```
public CellArea getRange(int index)
```


Ermittelt den von dieser Einstellung beeinflussten Bereich anhand des angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | der Index des Bereichs |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - return influenced range at given index.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isErrorCheck(int errorCheckType) {#isErrorCheck-int-}
```
public boolean isErrorCheck(int errorCheckType)
```


Prüft, ob der angegebene Fehlertyp überprüft wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). Fehlertyp kann überprüft werden |

**Returns:**
boolean - gibt true zurück, wenn der angegebene Fehlertyp überprüft wird (grünes Dreieck wird für die Zelle angezeigt, wenn die Prüfung fehlschlägt).
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeRange(int index) {#removeRange-int-}
```
public void removeRange(int index)
```


Entfernt einen Bereich anhand des angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | der Index des zu entfernenden Bereichs. |

### setErrorCheck(int errorCheckType, boolean isCheck) {#setErrorCheck-int-boolean-}
```
public void setErrorCheck(int errorCheckType, boolean isCheck)
```


Legt fest, ob der angegebene Fehlertyp überprüft wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). Fehlertyp kann überprüft werden. |
| isCheck | boolean | true, wenn der angegebene Fehlertyp überprüft werden muss (ein grünes Dreieck wird für die Zelle angezeigt, wenn die Überprüfung fehlgeschlagen ist). |

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

