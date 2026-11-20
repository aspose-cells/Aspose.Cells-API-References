---
title: "Validierung"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt data validation.settings dar."
type: docs
url: /de/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

Stellt data validation.settings dar.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Wendet die Validierung auf den Bereich an. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Wendet die Validierung auf den Bereich an. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Wendet die Validierung auf die angegebenen Bereiche an. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Validierung kopieren. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Stellt den Stil der Validierungswarnung dar. |
| [getAreas()](#getAreas--) | Ruft alle [CellArea](../../com.aspose.cells/cellarea) ab, die die Datenvalidierungseinstellungen enthalten. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [getErrorTitle()](#getErrorTitle--) | Stellt den Titel des Fehlermeldungsdialogs der Datenvalidierung dar. |
| [getFormula1()](#getFormula1--) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Liefert den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Liefert den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist. |
| [getFormula2()](#getFormula2--) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Liefert den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Liefert den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Gibt an, ob leere Werte durch die Datenvalidierung des Bereichs zulässig sind. |
| [getInCellDropDown()](#getInCellDropDown--) | Gibt an, ob die Datenvalidierung eine Dropdown-Liste mit zulässigen Werten anzeigt. |
| [getInputMessage()](#getInputMessage--) | Stellt die Eingabenachricht der Datenvalidierung dar. |
| [getInputTitle()](#getInputTitle--) | Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Ermittelt den Wert für die Listvalidierung der angegebenen Zelle. |
| [getOperator()](#getOperator--) | Stellt den Operator für die Datenvalidierung dar. |
| [getShowError()](#getShowError--) | Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt. |
| [getShowInput()](#getShowInput--) | Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Validierungsbereich auswählt. |
| [getType()](#getType--) | Stellt den Typ der Datenvalidierung dar. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Ermittelt den Validierungswert für die spezifische Zelle. |
| [getValue1()](#getValue1--) | Stellt den ersten mit der Datenvalidierung verknüpften Wert dar. |
| [getValue2()](#getValue2--) | Stellt den zweiten mit der Datenvalidierung verknüpften Wert dar. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Entfernt die Validierungseinstellungen in der Zelle. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Entfernt die Validierungseinstellungen im Bereich. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Entfernt diese Validierung aus den angegebenen Bereichen. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Stellt den Stil der Validierungswarnung dar. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Stellt die Fehlermeldung der Datenvalidierung dar. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Stellt den Titel des Fehlermeldungsdialogs der Datenvalidierung dar. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Gibt an, ob leere Werte durch die Datenvalidierung des Bereichs zulässig sind. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Gibt an, ob die Datenvalidierung eine Dropdown-Liste mit zulässigen Werten anzeigt. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Stellt die Eingabenachricht der Datenvalidierung dar. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Stellt den Titel des Eingabedialogfelds der Datenvalidierung dar. |
| [setOperator(int value)](#setOperator-int-) | Stellt den Operator für die Datenvalidierung dar. |
| [setShowError(boolean value)](#setShowError-boolean-) | Gibt an, ob die Fehlermeldung der Datenvalidierung angezeigt wird, wenn der Benutzer ungültige Daten eingibt. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Gibt an, ob die Eingabenachricht der Datenvalidierung angezeigt wird, wenn der Benutzer eine Zelle im Validierungsbereich auswählt. |
| [setType(int value)](#setType-int-) | Stellt den Typ der Datenvalidierung dar. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Stellt den ersten mit der Datenvalidierung verknüpften Wert dar. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Stellt den zweiten mit der Datenvalidierung verknüpften Wert dar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


Wendet die Validierung auf den Bereich an.

**Remarks**

Es ist gleichbedeutend mit der Verwendung von [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) unter Prüfung von Schnittmenge und Rand.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


Wendet die Validierung auf den Bereich an.

**Remarks**

In dieser Methode entfernen wir alle alten Validierungen im angegebenen Bereich. Für das linke obere Element der von Validation angewendeten Bereiche gilt: zuerst hat es die kleinste Startzeile, anschließend die kleinste Startspalte unter den Bereichen mit derselben kleinsten Startzeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich. |
| checkIntersection | boolean | Gibt an, ob die Schnittmenge des angegebenen Bereichs mit den Bereichen bestehender Validierungen geprüft wird. Wenn bereits eine Validierung im angegebenen Bereich (oder einem Teil davon) angewendet wurde, sollte die bestehende Validierung zunächst aus dem Bereich entfernt werden. Andernfalls kann es zu Beschädigungen der erzeugten Validierungen kommen. Wenn der Benutzer sicher ist, dass der hinzugefügte Bereich mit keinem bestehenden Bereich überschneidet, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |
| checkEdge | boolean | Gibt an, ob der Rand der von dieser Validierung angewendeten Bereiche geprüft wird. Die internen Einstellungen der Validierung hängen vom linken oberen Element ihrer angewendeten Bereiche ab; wird der angegebene Bereich zum neuen linken oberen Element, müssen die internen Einstellungen geändert und neu erstellt werden, sonst können unerwartete Ergebnisse auftreten. Wenn der Benutzer sicher ist, dass der hinzugefügte Bereich nicht das linke obere Element ist, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


Wendet die Validierung auf die angegebenen Bereiche an.

**Remarks**

In dieser Methode entfernen wir alle alten Validierungen im angegebenen Bereich. Für das linke obere Element der von Validation angewendeten Bereiche gilt: zuerst hat es die kleinste Startzeile, anschließend die kleinste Startspalte unter den Bereichen mit derselben kleinsten Startzeile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Die Bereiche. |
| checkIntersection | boolean | Ob die Schnittmenge des angegebenen Bereichs mit den Bereichen vorhandener Validierungen geprüft wird. Wenn eine Validierung im angegebenen Bereich (oder einem Teil davon) angewendet wurde, sollte die vorhandene Validierung zunächst aus dem angegebenen Bereich entfernt werden. Andernfalls kann es zu Beschädigungen der erzeugten Validierungen kommen. Wenn der Benutzer sicher ist, dass alle hinzugefügten Bereiche nicht mit einem bestehenden Bereich überschneiden, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |
| checkEdge | boolean | Ob die Kante der auf diese Validierung angewendeten Bereiche geprüft wird. Die internen Einstellungen der Validierung hängen vom oben‑links gelegenen ihrer angewendeten Bereiche ab, sodass wenn einer der angegebenen Bereiche zum neuen oben‑links gelegenen Bereich der angewendeten Bereiche wird, die internen Einstellungen geändert und neu aufgebaut werden sollten, andernfalls kann ein unerwartetes Ergebnis entstehen. Wenn der Benutzer sicher ist, dass keiner der hinzugefügten Bereiche oben‑links liegt, kann dieser Parameter aus Leistungsgründen auf false gesetzt werden. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


Validierung kopieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | Die Quellvalidierung. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | Die Kopieroption. |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


Stellt den Stil der Validierungswarnung dar.

Siehe [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Ruft alle [CellArea](../../com.aspose.cells/cellarea) ab, die die Datenvalidierungseinstellungen enthalten.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Liefert den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Liefert den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Liefert den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Liefert den Wert oder Ausdruck, der mit dieser Validierung für eine bestimmte Zelle verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | boolean | Ob die Formel gemäß der Gebietsschema formatiert werden muss. |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
java.lang.String - Der Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


Gibt an, ob leere Werte durch die Datenvalidierung des Bereichs zulässig sind.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


Gibt an, ob die Datenvalidierung eine Dropdown-Liste mit zulässigen Werten anzeigt.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Stellt die Eingabenachricht der Datenvalidierung dar.

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
java.lang.Object - Der Wert, um die Liste dieser Validierung für die angegebene Zelle zu erzeugen. Wenn die Liste auf einen Bereich verweist, wird der zurückgegebene Wert ein [ReferredArea](../../com.aspose.cells/referredarea)-Objekt sein; andernfalls kann der zurückgegebene Wert null, object[] oder ein einfaches Objekt sein.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Stellt den Operator für die Datenvalidierung dar.

Siehe [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
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
### getType() {#getType--}
```
public int getType()
```


Stellt den Typ der Datenvalidierung dar.

Siehe [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


Ermittelt den Validierungswert für die spezifische Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |
| isValue1 | boolean | Gibt an, ob der erste Wert abgerufen wird. |

**Returns:**
java.lang.Object -
### getValue1() {#getValue1--}
```
public Object getValue1()
```


Stellt den ersten mit der Datenvalidierung verknüpften Wert dar.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


Stellt den zweiten mit der Datenvalidierung verknüpften Wert dar.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


Entfernt die Validierungseinstellungen im Bereich.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | die Bereiche, in denen diese Validierungseinstellungen entfernt werden sollen. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


Entfernt diese Validierung aus den angegebenen Bereichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | die Bereiche, in denen diese Validierungseinstellungen entfernt werden sollen. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


Stellt den Stil der Validierungswarnung dar.

Siehe [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| isR1C1 | boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Stellt den Wert oder Ausdruck dar, der mit der Datenvalidierung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Setzt den Wert oder Ausdruck, der mit dieser Validierung verknüpft ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Der Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| isR1C1 | boolean | Ob die Formel eine R1C1-Formel ist. |
| isLocal | boolean | Ob die Formel lokalisierungsabhängig formatiert ist. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


Gibt an, ob leere Werte durch die Datenvalidierung des Bereichs zulässig sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


Gibt an, ob die Datenvalidierung eine Dropdown-Liste mit zulässigen Werten anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Stellt die Eingabenachricht der Datenvalidierung dar.

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

Siehe [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Stellt den Typ der Datenvalidierung dar.

Siehe [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


Stellt den ersten mit der Datenvalidierung verknüpften Wert dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


Stellt den zweiten mit der Datenvalidierung verknüpften Wert dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

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

