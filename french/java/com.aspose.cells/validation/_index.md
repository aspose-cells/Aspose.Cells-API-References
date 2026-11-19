---
title: "Validation"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente data validation.settings."
type: docs
url: /fr/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

Représente data validation.settings.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Applique la validation à la zone. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Applique la validation à la zone. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Applique la validation aux zones données. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Copier la validation. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Représente le style d'alerte de validation. |
| [getAreas()](#getAreas--) | Obtient toutes les [CellArea](../../com.aspose.cells/cellarea) qui contiennent les paramètres de validation des données. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Représente le message d'erreur de validation des données. |
| [getErrorTitle()](#getErrorTitle--) | Représente le titre de la boîte de dialogue d'erreur de validation des données. |
| [getFormula1()](#getFormula1--) | Représente la valeur ou l'expression associée à la validation des données. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Obtient la valeur ou l'expression associée à cette validation. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Obtient la valeur ou l'expression associée à cette validation pour une cellule spécifique. |
| [getFormula2()](#getFormula2--) | Représente la valeur ou l'expression associée à la validation des données. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Obtient la valeur ou l'expression associée à cette validation. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Obtient la valeur ou l'expression associée à cette validation pour une cellule spécifique. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Indique si les valeurs vides sont autorisées par la validation de données de la plage. |
| [getInCellDropDown()](#getInCellDropDown--) | Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables. |
| [getInputMessage()](#getInputMessage--) | Représente le message d'entrée de la validation des données. |
| [getInputTitle()](#getInputTitle--) | Représente le titre de la boîte de dialogue d'entrée de la validation des données. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Obtient la valeur de la liste de validation pour la cellule spécifiée. |
| [getOperator()](#getOperator--) | Représente l'opérateur de la validation des données. |
| [getShowError()](#getShowError--) | Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides. |
| [getShowInput()](#getShowInput--) | Indique si le message d'entrée de la validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données. |
| [getType()](#getType--) | Représente le type de validation des données. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Obtient la valeur de validation sur la cellule spécifique. |
| [getValue1()](#getValue1--) | Représente la première valeur associée à la validation des données. |
| [getValue2()](#getValue2--) | Représente la deuxième valeur associée à la validation des données. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Supprime les paramètres de validation dans la cellule. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Supprime les paramètres de validation dans la plage. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Supprime cette validation des zones spécifiées. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Représente le style d'alerte de validation. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Représente le message d'erreur de validation des données. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Représente le titre de la boîte de dialogue d'erreur de validation des données. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Représente la valeur ou l'expression associée à la validation des données. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Définit la valeur ou l'expression associée à cette validation. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Représente la valeur ou l'expression associée à la validation des données. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Définit la valeur ou l'expression associée à cette validation. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Indique si les valeurs vides sont autorisées par la validation de données de la plage. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Représente le message d'entrée de la validation des données. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Représente le titre de la boîte de dialogue d'entrée de la validation des données. |
| [setOperator(int value)](#setOperator-int-) | Représente l'opérateur de la validation des données. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indique si le message d'entrée de la validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données. |
| [setType(int value)](#setType-int-) | Représente le type de validation des données. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Représente la première valeur associée à la validation des données. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Représente la deuxième valeur associée à la validation des données. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


Applique la validation à la zone.

**Remarks**

C'est équivalent à utiliser [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) avec vérification de l'intersection et du bord.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | La zone. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


Applique la validation à la zone.

**Remarks**

Dans cette méthode, nous supprimerons toutes les anciennes validations dans la zone donnée. Pour la plage appliquée la plus en haut à gauche de Validation, d'abord sa StartRow est la plus petite, ensuite sa StartColumn est la plus petite parmi les zones qui ont la même plus petite StartRow.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | La zone. |
| checkIntersection | boolean | Indique s'il faut vérifier l'intersection de la zone donnée avec les zones des validations existantes. Si une validation a été appliquée dans la zone donnée (ou une partie de celle-ci), alors la validation existante doit d'abord être supprimée de la zone donnée. Sinon, une corruption peut être causée pour les validations générées. Si l'utilisateur est sûr que la zone ajoutée n'intersecte aucune zone existante, ce paramètre peut être défini sur false pour des considérations de performance. |
| checkEdge | boolean | Indique s'il faut vérifier le bord des zones appliquées de cette validation. Les paramètres internes de Validation dépendent de la zone la plus en haut à gauche de ses plages appliquées, donc si la zone donnée devient la nouvelle zone la plus en haut à gauche des plages appliquées, les paramètres internes doivent être modifiés et reconstruits, sinon un résultat inattendu peut survenir. Si l'utilisateur est sûr que la zone ajoutée n'est pas la zone la plus en haut à gauche, ce paramètre peut être défini sur false pour des considérations de performance. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


Applique la validation aux zones données.

**Remarks**

Dans cette méthode, nous supprimerons toutes les anciennes validations dans la zone donnée. Pour la plage appliquée la plus en haut à gauche de Validation, d'abord sa StartRow est la plus petite, ensuite sa StartColumn est la plus petite parmi les zones qui ont la même plus petite StartRow.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Les zones. |
| checkIntersection | boolean | Indique s'il faut vérifier l'intersection de la zone donnée avec les zones des validations existantes. Si une validation a été appliquée dans la zone donnée (ou une partie de celle-ci), alors la validation existante doit d'abord être supprimée de la zone donnée. Sinon, une corruption peut être causée pour les validations générées. Si l'utilisateur est sûr que toutes les zones ajoutées n'intersectent aucune zone existante, ce paramètre peut être défini sur false pour des considérations de performance. |
| checkEdge | boolean | Indique s'il faut vérifier le bord des zones appliquées de cette validation. Les paramètres internes de Validation dépendent de la zone la plus en haut à gauche de ses plages appliquées, donc si l'une des zones données devient la nouvelle zone la plus en haut à gauche des plages appliquées, les paramètres internes doivent être modifiés et reconstruits, sinon un résultat inattendu peut survenir. Si l'utilisateur est sûr qu'aucune des zones ajoutées n'est la zone la plus en haut à gauche, ce paramètre peut être défini sur false pour des considérations de performance. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


Copier la validation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | La validation source. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | L'option de copie. |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


Représente le style d'alerte de validation.

Voir [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Obtient toutes les [CellArea](../../com.aspose.cells/cellarea) qui contiennent les paramètres de validation des données.

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


Représente le message d'erreur de validation des données.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Représente le titre de la boîte de dialogue d'erreur de validation des données.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Représente la valeur ou l'expression associée à la validation des données.

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Obtient la valeur ou l'expression associée à cette validation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à cette validation.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtient la valeur ou l'expression associée à cette validation pour une cellule spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à cette validation.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Représente la valeur ou l'expression associée à la validation des données.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Obtient la valeur ou l'expression associée à cette validation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à cette validation.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Obtient la valeur ou l'expression associée à cette validation pour une cellule spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | boolean | Indique si la formule doit être formatée selon la locale. |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
java.lang.String - La valeur ou l'expression associée à cette validation.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


Indique si les valeurs vides sont autorisées par la validation de données de la plage.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Représente le message d'entrée de la validation des données.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Représente le titre de la boîte de dialogue d'entrée de la validation des données.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Obtient la valeur de la liste de validation pour la cellule spécifiée.

**Remarks**

Uniquement pour la validation dont le type est List et qui a été appliquée à la cellule donnée, sinon null sera retourné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
java.lang.Object - La valeur pour produire la liste de cette validation pour la cellule spécifiée. Si la liste fait référence à une plage, la valeur retournée sera un objet [ReferredArea](../../com.aspose.cells/referredarea) ; sinon la valeur retournée peut être null, object[], ou un objet simple.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Représente l'opérateur de la validation des données.

Voir [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Indique si le message d'entrée de la validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Représente le type de validation des données.

Voir [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


Obtient la valeur de validation sur la cellule spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |
| isValue1 | boolean | Indique si la première valeur est obtenue. |

**Returns:**
java.lang.Object -
### getValue1() {#getValue1--}
```
public Object getValue1()
```


Représente la première valeur associée à la validation des données.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


Représente la deuxième valeur associée à la validation des données.

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


Supprime les paramètres de validation dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


Supprime les paramètres de validation dans la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | les zones où ces paramètres de validation doivent être supprimés. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


Supprime cette validation des zones spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | les zones où ces paramètres de validation doivent être supprimés. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


Représente le style d'alerte de validation.

Voir [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Représente le message d'erreur de validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Représente le titre de la boîte de dialogue d'erreur de validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Représente la valeur ou l'expression associée à la validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Définit la valeur ou l'expression associée à cette validation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La valeur ou l'expression associée à cette condition de format. |
| isR1C1 | boolean | Indique si la formule est au format R1C1. |
| isLocal | boolean | Indique si la formule est formatée selon la locale. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Représente la valeur ou l'expression associée à la validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Définit la valeur ou l'expression associée à cette validation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La valeur ou l'expression associée à cette condition de format. |
| isR1C1 | boolean | Indique si la formule est au format R1C1. |
| isLocal | boolean | Indique si la formule est formatée selon la locale. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


Indique si les valeurs vides sont autorisées par la validation de données de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Représente le message d'entrée de la validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Représente le titre de la boîte de dialogue d'entrée de la validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Représente l'opérateur de la validation des données.

Voir [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Indique si le message d'entrée de la validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Représente le type de validation des données.

Voir [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


Représente la première valeur associée à la validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


Représente la deuxième valeur associée à la validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

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

