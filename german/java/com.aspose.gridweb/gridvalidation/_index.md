---
title: "GridValidation"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt data validation.settings dar."
type: docs
url: /de/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

Stellt data validation.settings dar.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ServerValidation](#ServerValidation) | Liest oder setzt den Namen der serverseitigen Validierungs‑JavaScript‑Funktion. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | Fügen Sie die Validierungseinstellungen in die Zelle ein. |
| [addACell(String cellname)](#addACell-java.lang.String-) | Fügen Sie die Validierungseinstellungen in die Zelle ein. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Wendet die Validierung auf den Bereich an. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Stellt eine Sammlung von [GridCellArea](../../com.aspose.gridweb/gridcellarea) dar, die die Datenvalidierungseinstellungen enthält. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | Liest den Namen der clientseitigen Validierungs‑JavaScript‑Funktion. |
| [getErrorMessage()](#getErrorMessage--) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [getErrorTitle()](#getErrorTitle--) | Stellt den Titel des Fehlermeldungsdialogs der Datenvalidierung dar. |
| [getFormula1()](#getFormula1--) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [getFormula2()](#getFormula2--) | Stellt den Wert oder Ausdruck dar, der mit dem zweiten Teil der Datenvalidierung verknüpft ist. |
| [getInputMessage()](#getInputMessage--) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [getInputTitle()](#getInputTitle--) | Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Ermittelt den Wert für die Listvalidierung der angegebenen Zelle. |
| [getOperator()](#getOperator--) | Stellt den Operator für die Datenvalidierung dar. |
| [getRegEx()](#getRegEx--) | Liest die reguläre Ausdruckszeichenfolge. |
| [getShowError()](#getShowError--) | Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt. |
| [getShowInput()](#getShowInput--) | Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Validierungsbereich auswählt. |
| [getValidationType()](#getValidationType--) | Liefert den Validierungstyp. |
| [getValue1()](#getValue1--) | Stellt den mit der Datenvalidierung verbundenen Wert dar. |
| [getValueList()](#getValueList--) | Liefert das Wertlisten-Objekt. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Liefert, ob der Zellenwert erforderlich ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Entfernt die Validierungseinstellungen in der Zelle. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Entfernt die Validierungseinstellungen im Bereich. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | Legt den Namen der JavaScript-Funktion für die Client-Validierung fest. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Stellt den Titel des Fehlermeldungsdialogs der Datenvalidierung dar. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Stellt den Wert oder Ausdruck dar, der mit dem zweiten Teil der Datenvalidierung verknüpft ist. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar. |
| [setOperator(int value)](#setOperator-int-) | Stellt den Operator für die Datenvalidierung dar. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Legt die reguläre Ausdruckszeichenfolge fest. |
| [setRequired(boolean value)](#setRequired-boolean-) | Legt fest, ob der Zellenwert erforderlich ist. |
| [setShowError(boolean value)](#setShowError-boolean-) | Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Validierungsbereich auswählt. |
| [setValidationType(int value)](#setValidationType-int-) | Legt den Validierungstyp fest. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Legt das Wertlisten-Objekt fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Liest oder setzt den Namen der serverseitigen Validierungs‑JavaScript‑Funktion.

**Remarks**

Verwenden Sie die Eigenschaft GridCustomServerValidation, um die serverseitige Validierung anzugeben.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


Fügen Sie die Validierungseinstellungen in die Zelle ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


Fügen Sie die Validierungseinstellungen in die Zelle ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellname | java.lang.String | Zellenname. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


Wendet die Validierung auf den Bereich an.

**Remarks**

In dieser Methode entfernen wir alle alten Validierungen in diesem Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


Stellt eine Sammlung von [GridCellArea](../../com.aspose.gridweb/gridcellarea) dar, die die Datenvalidierungseinstellungen enthält.

**Remarks**

Die alten Validierungen im Bereich werden nicht entfernt, wenn direkt etwas zu dieser Liste hinzugefügt wird.

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


Liest den Namen der clientseitigen Validierungs‑JavaScript‑Funktion.

**Remarks**

Verwenden Sie die Eigenschaft ClientValidationFunction, um den Namen der clientseitigen Validierungsfunktion anzugeben. Die Funktion sollte in dieser Form deklariert werden:
function customValicationFunction(source, value)
Der Parameter "source" ist das Zellenobjekt. Der Parameter "value" ist der Zeichenkettenwert einer zu prüfenden Zelle. Die Funktion sollte true zurückgeben, wenn der Wert gültig ist.

**Returns:**
java.lang.String
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


Stellt die Fehlermeldung der Datenvalidierung dar.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Stellt den Titel des Fehlermeldungsdialogs der Datenvalidierung dar.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist.

**Returns:**
java.lang.String
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Stellt den Wert oder Ausdruck dar, der mit dem zweiten Teil der Datenvalidierung verknüpft ist.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Stellt die Fehlermeldung der Datenvalidierung dar.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Ermittelt den Wert für die Listvalidierung der angegebenen Zelle.

**Remarks**

Nur für Validierungen, deren Typ List ist und die auf die angegebene Zelle angewendet wurden; andernfalls wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
java.lang.Object - Der Wert, um die Liste dieser Validierung für die angegebene Zelle zu erzeugen. Wenn die Liste auf einen Bereich verweist, wird der zurückgegebene Wert ein ReferredArea-Objekt sein; andernfalls kann der zurückgegebene Wert null, object[] oder ein einfacher Objekt sein.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Stellt den Operator für die Datenvalidierung dar.

Siehe [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


Liest die reguläre Ausdruckszeichenfolge.

**Returns:**
java.lang.String
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Validierungsbereich auswählt.

**Returns:**
boolean
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


Liefert den Validierungstyp.

Siehe [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


Stellt den mit der Datenvalidierung verbundenen Wert dar.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


Liefert das Wertlisten-Objekt.

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


Liefert, ob der Zellenwert erforderlich ist.

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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Entfernt die Validierungseinstellungen in der Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


Entfernt die Validierungseinstellungen im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich, der die Datenvalidierungseinstellungen enthält. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


Legt den Namen der JavaScript-Funktion für die Client-Validierung fest.

**Remarks**

Verwenden Sie die Eigenschaft ClientValidationFunction, um den Namen der clientseitigen Validierungsfunktion anzugeben. Die Funktion sollte in dieser Form deklariert werden:
function customValicationFunction(source, value)
Der Parameter "source" ist das Zellenobjekt. Der Parameter "value" ist der Zeichenkettenwert einer zu prüfenden Zelle. Die Funktion sollte true zurückgeben, wenn der Wert gültig ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Stellt die Fehlermeldung der Datenvalidierung dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Stellt den Titel des Fehlermeldungsdialogs der Datenvalidierung dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Stellt den Wert oder Ausdruck dar, der mit dem zweiten Teil der Datenvalidierung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Stellt die Fehlermeldung der Datenvalidierung dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Stellt den Operator für die Datenvalidierung dar.

Siehe [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


Legt die reguläre Ausdruckszeichenfolge fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


Legt fest, ob der Zellenwert erforderlich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Validierungsbereich auswählt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


Legt den Validierungstyp fest.

Siehe [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


Legt das Wertlisten-Objekt fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.ArrayList<java.lang.String> |  |

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

