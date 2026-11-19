---
title: "GridValidation"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente data validation.settings."
type: docs
url: /fr/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

Représente data validation.settings.
## Champs

| Champ | Description |
| --- | --- |
| [ServerValidation](#ServerValidation) | Obtient ou définit le nom de la fonction JavaScript de validation côté serveur. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | ajoutez les paramètres de validation dans la cellule. |
| [addACell(String cellname)](#addACell-java.lang.String-) | ajoutez les paramètres de validation dans la cellule. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Applique la validation à la zone. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Représente une collection de [GridCellArea](../../com.aspose.gridweb/gridcellarea) qui contient les paramètres de validation des données. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | Obtient le nom de la fonction JavaScript de validation côté client. |
| [getErrorMessage()](#getErrorMessage--) | Représente le message d'erreur de validation des données. |
| [getErrorTitle()](#getErrorTitle--) | Représente le titre de la boîte de dialogue d'erreur de validation des données. |
| [getFormula1()](#getFormula1--) | Représente la valeur ou l'expression associée à la validation des données. |
| [getFormula2()](#getFormula2--) | Représente la valeur ou l'expression associée à la deuxième partie de la validation des données. |
| [getInputMessage()](#getInputMessage--) | Représente le message d'erreur de validation des données. |
| [getInputTitle()](#getInputTitle--) | Représente le titre de la boîte de dialogue d'entrée de la validation des données. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Obtient la valeur de la liste de validation pour la cellule spécifiée. |
| [getOperator()](#getOperator--) | Représente l'opérateur de la validation des données. |
| [getRegEx()](#getRegEx--) | Obtient la chaîne d'expression régulière. |
| [getShowError()](#getShowError--) | Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides. |
| [getShowInput()](#getShowInput--) | Indique si le message d'entrée de la validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données. |
| [getValidationType()](#getValidationType--) | Obtient le type de validation. |
| [getValue1()](#getValue1--) | Représente la valeur associée à la validation des données. |
| [getValueList()](#getValueList--) | Obtient l'objet de liste de valeurs. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Obtient si la valeur de la cellule est requise. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Supprime les paramètres de validation dans la cellule. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Supprime les paramètres de validation dans la plage. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | Définit le nom de la fonction JavaScript de validation côté client. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Représente le message d'erreur de validation des données. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Représente le titre de la boîte de dialogue d'erreur de validation des données. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Représente la valeur ou l'expression associée à la validation des données. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Représente la valeur ou l'expression associée à la deuxième partie de la validation des données. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Représente le message d'erreur de validation des données. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Représente le titre de la boîte de dialogue d'entrée de la validation des données. |
| [setOperator(int value)](#setOperator-int-) | Représente l'opérateur de la validation des données. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Définit la chaîne d'expression régulière. |
| [setRequired(boolean value)](#setRequired-boolean-) | Définit si la valeur de la cellule est requise. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indique si le message d'entrée de la validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données. |
| [setValidationType(int value)](#setValidationType-int-) | Définit le type de validation. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Définit l'objet de liste de valeurs. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Obtient ou définit le nom de la fonction JavaScript de validation côté serveur.

**Remarks**

Utilisez la propriété GridCustomServerValidation pour spécifier la validation côté serveur.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


ajoutez les paramètres de validation dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


ajoutez les paramètres de validation dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellname | java.lang.String | nom de cellule. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


Applique la validation à la zone.

**Remarks**

Dans cette méthode, nous supprimerons toutes les anciennes validations sur cette zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La zone. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


Représente une collection de [GridCellArea](../../com.aspose.gridweb/gridcellarea) qui contient les paramètres de validation des données.

**Remarks**

Les anciennes validations sur la zone ne seront pas supprimées si elles sont ajoutées directement à cette liste.

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


Obtient le nom de la fonction JavaScript de validation côté client.

**Remarks**

Utilisez la propriété ClientValidationFunction pour spécifier le nom de la fonction de validation côté client. La fonction doit être déclarée de cette manière :
function customValicationFunction(source, value)
Le paramètre "source" est l'objet cellule. Le paramètre "value" est la valeur chaîne d'une cellule à vérifier. La fonction doit renvoyer true si la valeur est valide.

**Returns:**
java.lang.String
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
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Représente la valeur ou l'expression associée à la deuxième partie de la validation des données.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Représente le message d'erreur de validation des données.

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
java.lang.Object - La valeur pour produire la liste de cette validation pour la cellule spécifiée. Si la liste fait référence à une plage, alors la valeur retournée sera un objet ReferredArea ; sinon la valeur retournée peut être null, object[], ou un objet simple.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Représente l'opérateur de la validation des données.

Voir [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


Obtient la chaîne d'expression régulière.

**Returns:**
java.lang.String
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
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


Obtient le type de validation.

Voir [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


Représente la valeur associée à la validation des données.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


Obtient l'objet de liste de valeurs.

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


Obtient si la valeur de la cellule est requise.

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


Supprime les paramètres de validation dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


Supprime les paramètres de validation dans la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | La plage qui contient les paramètres de validation des données. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


Définit le nom de la fonction JavaScript de validation côté client.

**Remarks**

Utilisez la propriété ClientValidationFunction pour spécifier le nom de la fonction de validation côté client. La fonction doit être déclarée de cette manière :
function customValicationFunction(source, value)
Le paramètre "source" est l'objet cellule. Le paramètre "value" est la valeur chaîne d'une cellule à vérifier. La fonction doit renvoyer true si la valeur est valide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Représente la valeur ou l'expression associée à la deuxième partie de la validation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Représente le message d'erreur de validation des données.

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

Voir [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


Définit la chaîne d'expression régulière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


Définit si la valeur de la cellule est requise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


Définit le type de validation.

Voir [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


Définit l'objet de liste de valeurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.ArrayList<java.lang.String> |  |

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

