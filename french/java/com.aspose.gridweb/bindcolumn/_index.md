---
title: "BindColumn"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "BindColumn."
type: docs
url: /fr/java/com.aspose.gridweb/bindcolumn/
---

**Inheritance:**
java.lang.Object
```
public class BindColumn
```

BindColumn.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [BindColumn()](#BindColumn--) | Constructeur par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeStyle()](#getAlternativeStyle--) | Obtient le style alternatif de la colonne. |
| [getCaption()](#getCaption--) | La légende de la colonne. |
| [getClass()](#getClass--) |  |
| [getColumnHeaderStyle()](#getColumnHeaderStyle--) | Obtient le style de la colonne. |
| [getCommandName()](#getCommandName--) | Le nom de commande de la colonne. |
| [getCommandText()](#getCommandText--) | Le texte de commande affiché de la colonne. |
| [getCustomFormat()](#getCustomFormat--) | La chaîne de format personnalisée. |
| [getDataField()](#getDataField--) | Obtient la chaîne du nom du champ de données. |
| [getEnableSort()](#getEnableSort--) | Indique si l'utilisateur peut cliquer sur l'en-tête de la colonne pour trier par ce champ. |
| [getImageUrl()](#getImageUrl--) | L'URL de l'image du lien hypertexte de commande. |
| [getName()](#getName--) | Utilisé uniquement au moment de la conception. |
| [getNumberType()](#getNumberType--) | Obtient le type numérique de la colonne. |
| [getStyle()](#getStyle--) | Obtient le style de la colonne. |
| [getUseAlternativeStyle()](#getUseAlternativeStyle--) | Obtient si le style alternatif doit être utilisé pour la colonne. |
| [getValidation()](#getValidation--) | Obtient l'objet de validation de la colonne. |
| [getWidth()](#getWidth--) | Obtient ou définit la largeur de la colonne. Seuls les pixels ou les points sont acceptés. |
| [hashCode()](#hashCode--) |  |
| [isAutoCreated()](#isAutoCreated--) | Indique si la colonne est créée automatiquement. |
| [isReadOnly()](#isReadOnly--) | Indique si la colonne est en lecture seule. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlternativeStyle(GridTableItemStyle value)](#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-) | Définit le style alternatif de la colonne. |
| [setAutoCreated(boolean value)](#setAutoCreated-boolean-) | Indique si la colonne est créée automatiquement. |
| [setCaption(String value)](#setCaption-java.lang.String-) | La légende de la colonne. |
| [setColumnHeaderStyle(GridTableItemStyle value)](#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-) | Définit le style de la colonne. |
| [setCommandName(String value)](#setCommandName-java.lang.String-) | Le nom de commande de la colonne. |
| [setCommandText(String value)](#setCommandText-java.lang.String-) | Le texte de commande affiché de la colonne. |
| [setCustomFormat(String value)](#setCustomFormat-java.lang.String-) | La chaîne de format personnalisée. |
| [setDataField(String value)](#setDataField-java.lang.String-) | Définit la chaîne du nom du champ de données. |
| [setEnableSort(boolean value)](#setEnableSort-boolean-) | Indique si l'utilisateur peut cliquer sur l'en-tête de la colonne pour trier par ce champ. |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | L'URL de l'image du lien hypertexte de commande. |
| [setNumberType(int value)](#setNumberType-int-) | Définit le type numérique de la colonne. |
| [setReadOnly(boolean value)](#setReadOnly-boolean-) | Indique si la colonne est en lecture seule. |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Définit le style de la colonne. |
| [setUseAlternativeStyle(boolean value)](#setUseAlternativeStyle-boolean-) | Définit si le style alternatif doit être utilisé pour la colonne. |
| [setValidation(GridValidation value)](#setValidation-com.aspose.gridweb.GridValidation-) | Définit l'objet de validation de la colonne. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Obtient ou définit la largeur de la colonne. Seuls les pixels ou les points sont acceptés. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BindColumn() {#BindColumn--}
```
public BindColumn()
```


Constructeur par défaut.

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
### getAlternativeStyle() {#getAlternativeStyle--}
```
public GridTableItemStyle getAlternativeStyle()
```


Obtient le style alternatif de la colonne.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCaption() {#getCaption--}
```
public String getCaption()
```


La légende de la colonne.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnHeaderStyle() {#getColumnHeaderStyle--}
```
public GridTableItemStyle getColumnHeaderStyle()
```


Obtient le style de la colonne.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCommandName() {#getCommandName--}
```
public String getCommandName()
```


Le nom de commande de la colonne. Un lien hypertexte CellCommand sera créé dans la cellule liée si la propriété CommandName est définie.

**Returns:**
java.lang.String
### getCommandText() {#getCommandText--}
```
public String getCommandText()
```


Le texte de commande affiché de la colonne. Si défini sur null, la cellule utilisera la valeur du champ comme texte de commande.

**Returns:**
java.lang.String
### getCustomFormat() {#getCustomFormat--}
```
public String getCustomFormat()
```


La chaîne de format personnalisée.

**Returns:**
java.lang.String
### getDataField() {#getDataField--}
```
public String getDataField()
```


Obtient la chaîne du nom du champ de données.

**Returns:**
java.lang.String
### getEnableSort() {#getEnableSort--}
```
public boolean getEnableSort()
```


Indique si l'utilisateur peut cliquer sur l'en-tête de la colonne pour trier par ce champ.

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


L'URL de l'image du lien hypertexte de commande.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Utilisé uniquement au moment de la conception.

**Returns:**
java.lang.String
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Obtient le type numérique de la colonne.

Voir [NumberType](../../com.aspose.gridweb/numbertype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Obtient le style de la colonne.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUseAlternativeStyle() {#getUseAlternativeStyle--}
```
public boolean getUseAlternativeStyle()
```


Obtient si le style alternatif doit être utilisé pour la colonne.

**Returns:**
boolean
### getValidation() {#getValidation--}
```
public GridValidation getValidation()
```


Obtient l'objet de validation de la colonne.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Obtient ou définit la largeur de la colonne. Seuls les pixels ou les points sont acceptés.

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoCreated() {#isAutoCreated--}
```
public boolean isAutoCreated()
```


Indique si la colonne est créée automatiquement. Si vrai, la colonne sera supprimée lorsque l'utilisateur modifie la source de données au moment de la conception.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Indique si la colonne est en lecture seule.

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




### setAlternativeStyle(GridTableItemStyle value) {#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setAlternativeStyle(GridTableItemStyle value)
```


Définit le style alternatif de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoCreated(boolean value) {#setAutoCreated-boolean-}
```
public void setAutoCreated(boolean value)
```


Indique si la colonne est créée automatiquement. Si vrai, la colonne sera supprimée lorsque l'utilisateur modifie la source de données au moment de la conception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


La légende de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setColumnHeaderStyle(GridTableItemStyle value) {#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setColumnHeaderStyle(GridTableItemStyle value)
```


Définit le style de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setCommandName(String value) {#setCommandName-java.lang.String-}
```
public void setCommandName(String value)
```


Le nom de commande de la colonne. Un lien hypertexte CellCommand sera créé dans la cellule liée si la propriété CommandName est définie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCommandText(String value) {#setCommandText-java.lang.String-}
```
public void setCommandText(String value)
```


Le texte de commande affiché de la colonne. Si défini sur null, la cellule utilisera la valeur du champ comme texte de commande.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCustomFormat(String value) {#setCustomFormat-java.lang.String-}
```
public void setCustomFormat(String value)
```


La chaîne de format personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDataField(String value) {#setDataField-java.lang.String-}
```
public void setDataField(String value)
```


Définit la chaîne du nom du champ de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setEnableSort(boolean value) {#setEnableSort-boolean-}
```
public void setEnableSort(boolean value)
```


Indique si l'utilisateur peut cliquer sur l'en-tête de la colonne pour trier par ce champ.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


L'URL de l'image du lien hypertexte de commande.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Définit le type numérique de la colonne.

Voir [NumberType](../../com.aspose.gridweb/numbertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setReadOnly(boolean value) {#setReadOnly-boolean-}
```
public void setReadOnly(boolean value)
```


Indique si la colonne est en lecture seule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Définit le style de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setUseAlternativeStyle(boolean value) {#setUseAlternativeStyle-boolean-}
```
public void setUseAlternativeStyle(boolean value)
```


Définit si le style alternatif doit être utilisé pour la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setValidation(GridValidation value) {#setValidation-com.aspose.gridweb.GridValidation-}
```
public void setValidation(GridValidation value)
```


Définit l'objet de validation de la colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridValidation](../../com.aspose.gridweb/gridvalidation) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Obtient ou définit la largeur de la colonne. Seuls les pixels ou les points sont acceptés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

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

