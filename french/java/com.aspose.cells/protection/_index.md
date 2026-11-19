---
title: "Protection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les différents types d'options de protection disponibles pour une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Représente les différents types d'options de protection disponibles pour une feuille de calcul.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Copier les informations de protection. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Représente si la suppression de colonnes est autorisée sur une feuille protégée. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Représente si la suppression de lignes est autorisée sur une feuille protégée. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille protégée. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille protégée. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille protégée. |
| [getAllowFiltering()](#getAllowFiltering--) | Représente si l'utilisateur est autorisé à utiliser un AutoFilter créé avant la protection de la feuille. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Représente si le formatage des cellules est autorisé sur une feuille protégée. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Représente si le formatage des colonnes est autorisé sur une feuille protégée |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Représente si le formatage des lignes est autorisé sur une feuille protégée |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Représente si l'insertion de colonnes est autorisée sur une feuille protégée |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Représente si l'insertion d'hyperliens est autorisée sur une feuille de calcul protégée |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Représente si l'utilisateur est autorisé à sélectionner des cellules verrouillées sur une feuille de calcul protégée. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Représente si l'utilisateur est autorisé à sélectionner des cellules déverrouillées sur une feuille de calcul protégée. |
| [getAllowSorting()](#getAllowSorting--) | Représente si l'option de tri est autorisée sur une feuille de calcul protégée. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Représente le mot de passe pour protéger la feuille de calcul. |
| [getPasswordHash()](#getPasswordHash--) | Obtient le hachage du mot de passe actuel. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indique si la feuille de calcul est protégée par un mot de passe. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Représente si la suppression de colonnes est autorisée sur une feuille protégée. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Représente si la suppression de lignes est autorisée sur une feuille protégée. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille protégée. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille protégée. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille protégée. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Représente si l'utilisateur est autorisé à utiliser un AutoFilter créé avant la protection de la feuille. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Représente si le formatage des cellules est autorisé sur une feuille protégée. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Représente si le formatage des colonnes est autorisé sur une feuille protégée |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Représente si le formatage des lignes est autorisé sur une feuille protégée |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Représente si l'insertion de colonnes est autorisée sur une feuille protégée |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Représente si l'insertion d'hyperliens est autorisée sur une feuille de calcul protégée |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Représente si l'utilisateur est autorisé à sélectionner des cellules verrouillées sur une feuille de calcul protégée. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Représente si l'utilisateur est autorisé à sélectionner des cellules déverrouillées sur une feuille de calcul protégée. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Représente si l'option de tri est autorisée sur une feuille de calcul protégée. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Représente le mot de passe pour protéger la feuille de calcul. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Vérifie le mot de passe. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Copier les informations de protection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Représente si la suppression de colonnes est autorisée sur une feuille protégée.

**Remarks**

Les colonnes contenant les cellules à supprimer doivent être déverrouillées lorsque la feuille est protégée, et l'option "Sélectionner les cellules déverrouillées" doit être activée.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Représente si la suppression de lignes est autorisée sur une feuille protégée.

**Remarks**

Les lignes contenant les cellules à supprimer doivent être déverrouillées lorsque la feuille est protégée, et l'option "Sélectionner les cellules déverrouillées" doit être activée.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille protégée.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille protégée.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille protégée.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Représente si l'utilisateur est autorisé à utiliser un AutoFilter créé avant la protection de la feuille.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Représente si le formatage des cellules est autorisé sur une feuille protégée.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Représente si le formatage des colonnes est autorisé sur une feuille protégée

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Représente si le formatage des lignes est autorisé sur une feuille protégée

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Représente si l'insertion de colonnes est autorisée sur une feuille protégée

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Représente si l'insertion d'hyperliens est autorisée sur une feuille de calcul protégée

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Représente si l'utilisateur est autorisé à sélectionner des cellules verrouillées sur une feuille de calcul protégée.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Représente si l'utilisateur est autorisé à sélectionner des cellules déverrouillées sur une feuille de calcul protégée.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Représente si l'option de tri est autorisée sur une feuille de calcul protégée.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée.

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


Représente le mot de passe pour protéger la feuille de calcul.

**Remarks**

Si le mot de passe est défini sur null ou une chaîne vide, vous pouvez déprotéger la feuille de calcul ou le classeur sans utiliser de mot de passe. Sinon, vous devez spécifier le mot de passe pour déprotéger la feuille de calcul ou le classeur.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Obtient le hachage du mot de passe actuel.

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


Indique si la feuille de calcul est protégée par un mot de passe.

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


Représente si la suppression de colonnes est autorisée sur une feuille protégée.

**Remarks**

Les colonnes contenant les cellules à supprimer doivent être déverrouillées lorsque la feuille est protégée, et l'option "Sélectionner les cellules déverrouillées" doit être activée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


Représente si la suppression de lignes est autorisée sur une feuille protégée.

**Remarks**

Les lignes contenant les cellules à supprimer doivent être déverrouillées lorsque la feuille est protégée, et l'option "Sélectionner les cellules déverrouillées" doit être activée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


Représente si l'utilisateur est autorisé à modifier le contenu des cellules verrouillées sur une feuille protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


Représente si l'utilisateur est autorisé à manipuler les objets de dessin sur une feuille protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


Représente si l'utilisateur est autorisé à modifier les scénarios sur une feuille protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


Représente si l'utilisateur est autorisé à utiliser un AutoFilter créé avant la protection de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


Représente si le formatage des cellules est autorisé sur une feuille protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


Représente si le formatage des colonnes est autorisé sur une feuille protégée

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


Représente si le formatage des lignes est autorisé sur une feuille protégée

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


Représente si l'insertion de colonnes est autorisée sur une feuille protégée

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


Représente si l'insertion d'hyperliens est autorisée sur une feuille de calcul protégée

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


Représente si l'insertion de lignes est autorisée sur une feuille de calcul protégée

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


Représente si l'utilisateur est autorisé à sélectionner des cellules verrouillées sur une feuille de calcul protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


Représente si l'utilisateur est autorisé à sélectionner des cellules déverrouillées sur une feuille de calcul protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


Représente si l'option de tri est autorisée sur une feuille de calcul protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


Représente si l'utilisateur est autorisé à manipuler les tableaux croisés dynamiques sur une feuille de calcul protégée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Représente le mot de passe pour protéger la feuille de calcul.

**Remarks**

Si le mot de passe est défini sur null ou une chaîne vide, vous pouvez déprotéger la feuille de calcul ou le classeur sans utiliser de mot de passe. Sinon, vous devez spécifier le mot de passe pour déprotéger la feuille de calcul ou le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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


Vérifie le mot de passe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Le mot de passe. |

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

