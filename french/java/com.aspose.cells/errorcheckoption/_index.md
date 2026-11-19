---
title: "ErrorCheckOption"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Paramètre de vérification d'erreur appliqué à certaines plages."
type: docs
url: /fr/java/com.aspose.cells/errorcheckoption/
---

**Inheritance:**
java.lang.Object
```
public class ErrorCheckOption
```

Paramètre de vérification d'erreur appliqué à certaines plages.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [addRange(CellArea ca)](#addRange-com.aspose.cells.CellArea-) | Ajoute une plage influencée par ce paramètre. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCountOfRange()](#getCountOfRange--) | Obtient le nombre de plages influencées par ce paramètre. |
| [getRange(int index)](#getRange-int-) | Obtient la plage influencée de ce paramètre par l'index donné. |
| [hashCode()](#hashCode--) |  |
| [isErrorCheck(int errorCheckType)](#isErrorCheck-int-) | Vérifie si le type d'erreur donné sera vérifié. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeRange(int index)](#removeRange-int-) | Supprime une plage par l'index donné. |
| [setErrorCheck(int errorCheckType, boolean isCheck)](#setErrorCheck-int-boolean-) | Définit si le type d'erreur donné sera vérifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(CellArea ca) {#addRange-com.aspose.cells.CellArea-}
```
public int addRange(CellArea ca)
```


Ajoute une plage influencée par ce paramètre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | la plage à ajouter. |

**Returns:**
int - l'index de la plage ajoutée dans la liste des plages de ce paramètre.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
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


Obtient le nombre de plages influencées par ce paramètre.

**Returns:**
int - le nombre de plages influencées par ce paramètre.
### getRange(int index) {#getRange-int-}
```
public CellArea getRange(int index)
```


Obtient la plage influencée de ce paramètre par l'index donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index de la plage |

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


Vérifie si le type d'erreur donné sera vérifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). le type d'erreur peut être vérifié |

**Returns:**
booléen - renvoie true si le type d'erreur donné sera vérifié (un triangle vert sera affiché pour la cellule si la vérification échoue).
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


Supprime une plage par l'index donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | l'index de la plage à supprimer. |

### setErrorCheck(int errorCheckType, boolean isCheck) {#setErrorCheck-int-boolean-}
```
public void setErrorCheck(int errorCheckType, boolean isCheck)
```


Définit si le type d'erreur donné sera vérifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). le type d'erreur peut être vérifié. |
| isCheck | boolean | true si le type d'erreur donné doit être vérifié (un triangle vert sera affiché pour la cellule si la vérification échoue). |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

