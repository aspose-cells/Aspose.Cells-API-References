---
title: "GridCell"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un objet cellule."
type: docs
url: /fr/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

Représente un objet cellule.
## Méthodes

| Méthode | Description |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Indique si cette cellule contient un lien externe. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Copie les données d'une cellule source. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | copier le style et définir le style pour la cellule |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Crée un objet commentaire pour une cellule. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Crée un objet de validation pour une cellule. |
| [equals(Object obj)](#equals-java.lang.Object-) | Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule. |
| [getBoolValue()](#getBoolValue--) | Obtient la valeur booléenne contenue dans la cellule. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient le numéro de colonne (indexé à zéro) de la cellule. |
| [getComment()](#getComment--) | Obtenir l'objet commentaire sur cette cellule |
| [getDateValue()](#getDateValue--) | Obtient la valeur DateTime contenue dans la cellule. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Obtient la valeur chaîne formatée de cette cellule. |
| [getDoubleValue()](#getDoubleValue--) | Obtient la valeur double contenue dans la cellule. |
| [getFloatValue()](#getFloatValue--) | Obtient la valeur float contenue dans la cellule. |
| [getFormula()](#getFormula--) | Obtient une formule du [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | Obtient la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [getIntValue()](#getIntValue--) | Obtient la valeur entière contenue dans la cellule. |
| [getName()](#getName--) | Obtient le nom de la cellule. |
| [getRow()](#getRow--) | Obtient le numéro de ligne (indexé à zéro) de la cellule. |
| [getStringValue()](#getStringValue--) | Obtient la valeur chaîne contenue dans la cellule. |
| [getStyle()](#getStyle--) | Obtient la copie du style de la cellule. définir le style pour la cellule. |
| [getType()](#getType--) | renvoie le type de valeur de la cellule, la signification peut être consultée dans GridCellValueType.java |
| [getValue()](#getValue--) | Obtient la valeur contenue dans cette cellule. |
| [getWidthOfValue()](#getWidthOfValue--) | Obtient la largeur de la valeur en pixels. |
| [hashCode()](#hashCode--) | Servir de fonction de hachage pour un type particulier. |
| [isErrorValue()](#isErrorValue--) | Vérifie si une formule peut correctement évaluer un résultat. |
| [isFormula()](#isFormula--) | Indique si la cellule spécifiée contient une formule. |
| [isStyleSet()](#isStyleSet--) | Indique si le style de la cellule est défini. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Place une valeur booléenne dans la cellule. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Place une valeur DateTime dans la cellule. |
| [putValue(double param_double)](#putValue-double-) | Place une valeur double dans la cellule. |
| [putValue(int param_int)](#putValue-int-) | Place une valeur int dans la cellule. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Place une valeur d'objet dans la cellule. même que setValue(Object param\_object) |
| [putValue(String param_string)](#putValue-java.lang.String-) | Place une valeur String dans la cellule. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Insère une valeur dans la cellule, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Définit la valeur de la cellule avec une valeur chaîne et définit le format de la cellule selon cette valeur. |
| [removeComment()](#removeComment--) | Supprime l'objet commentaire de la cellule. |
| [removeValidation()](#removeValidation--) | Supprime l'objet de validation de la cellule. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Définit les bordures (haut, bas, gauche et droite) pour une cellule, toutes les bordures ont le même style de bordure. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | définit le format personnalisé, null ou chaîne vide signifie aucun format personnalisé. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Définit une formule du [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Définir la formule et la valeur de la formule. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Définit la chaîne HTML qui contient des données et certains formats dans cette cellule. |
| [setNumberType(int numbertype)](#setNumberType-int-) | définir le format d'affichage des nombres et des dates |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Obtient la copie du style de la cellule. définir le style pour la cellule. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Obtient la valeur contenue dans cette cellule. |
| [toString()](#toString--) | Renvoie une chaîne qui représente l'objet Cell actuel. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Indique si cette cellule contient un lien externe. S'applique uniquement lorsque la cellule est une cellule de formule.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


Copie les données d'une cellule source.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Objet source [GridCell](../../com.aspose.gridweb/gridcell). |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


copier le style et définir le style pour la cellule

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Le style source. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


Crée un objet commentaire pour une cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| note | java.lang.String | note de commentaire. |
| auteur | java.lang.String | auteur du commentaire. |
| isvisible | boolean | si le commentaire est visible. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


Crée un objet de validation pour une cellule.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Type de validation. |
| isRequried | boolean | Si la valeur de la cellule est requise. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Vérifie si cet objet fait référence à la même cellule qu'un autre objet cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | un autre objet GridCell |

**Returns:**
booléen - vrai si deux objets cellule font référence à la même cellule.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Obtient la valeur booléenne contenue dans la cellule.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtient le numéro de colonne (indexé à zéro) de la cellule.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


Obtenir l'objet commentaire sur cette cellule

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


Obtient la valeur DateTime contenue dans la cellule.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Obtient la valeur chaîne formatée de cette cellule.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Obtient la valeur double contenue dans la cellule.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Obtient la valeur float contenue dans la cellule.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtient une formule du [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Une chaîne de formule commence toujours par un signe égal (=). Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, par exemple "=SUM(A1, E1, H2)".

L'utilisateur peut définir n'importe quelle formule dans le fichier de conception du Workbook. Aspose.Cells conservera toutes les formules. Si l'utilisateur utilise cette propriété pour définir une formule dans une cellule, la majeure partie des fonctions intégrées du Workbook est prise en charge. Et davantage arrive. Si vous avez des besoins spécifiques concernant les fonctions intégrées du Workbook, veuillez nous le faire savoir.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Obtient la chaîne HTML qui contient des données et certains formats dans cette cellule.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Obtient la valeur entière contenue dans la cellule.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la cellule. Par exemple : A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Obtient le numéro de ligne (indexé à zéro) de la cellule.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtient la valeur chaîne contenue dans la cellule.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Obtient la copie du style de la cellule. définir le style pour la cellule.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


renvoie le type de valeur de la cellule, la signification peut être consultée dans GridCellValueType.java

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient la valeur contenue dans cette cellule.

**Remarks**

Type possible :

null,

Boolean,

DateTime,

Double,

Integer

String.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Obtient la largeur de la valeur en pixels.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


Servir de fonction de hachage pour un type particulier.

**Returns:**
int - Un code de hachage pour l'objet GridCell actuel.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Vérifie si une formule peut correctement évaluer un résultat.

**Remarks**

S'applique uniquement à la cellule de formule.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Indique si la cellule spécifiée contient une formule.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indique si le style de la cellule est défini. Si la valeur retournée est false, cela signifie que cette cellule possède le format de cellule par défaut.

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




### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```


Place une valeur booléenne dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| param_boolean | boolean | Valeur d'entrée |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


Place une valeur DateTime dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Valeur d'entrée |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


Place une valeur double dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| param_double | double | Valeur d'entrée |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


Place une valeur int dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| param_int | int | Valeur d'entrée |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Place une valeur d'objet dans la cellule. même que setValue(Object param\_object)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| objectValue | java.lang.Object | valeur d'entrée |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


Place une valeur String dans la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| param_string | java.lang.String | Valeur d'entrée |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Place une valeur chaîne dans la cellule et convertit la valeur en un autre type de données si approprié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Valeur d'entrée |
| isConverted | boolean | True : converti en un autre type de données si approprié. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Insère une valeur dans la cellule, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Valeur d'entrée |
| isConverted | boolean | True : converti en un autre type de données si approprié. |
| setStyle | boolean | True : définir le format numérique dans le style de la cellule lors de la conversion en un autre type de données |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


Définit la valeur de la cellule avec une valeur chaîne et définit le format de la cellule selon cette valeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Valeur d'entrée. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


Supprime l'objet commentaire de la cellule.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


Supprime l'objet de validation de la cellule.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


Définit les bordures (haut, bas, gauche et droite) pour une cellule, toutes les bordures ont le même style de bordure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Le style de la bordure. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


définit le format personnalisé, null ou chaîne vide signifie aucun format personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| personnalisé | java.lang.String | la présentation de chaîne personnalisée |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Définit une formule du [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Une chaîne de formule commence toujours par un signe égal (=). Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, par exemple "=SUM(A1, E1, H2)".

L'utilisateur peut définir n'importe quelle formule dans le fichier de conception du Workbook. Aspose.Cells conservera toutes les formules. Si l'utilisateur utilise cette propriété pour définir une formule dans une cellule, la majeure partie des fonctions intégrées du Workbook est prise en charge. Et davantage arrive. Si vous avez des besoins spécifiques concernant les fonctions intégrées du Workbook, veuillez nous le faire savoir.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Définir la formule et la valeur de la formule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | La formule. |
| valeur | java.lang.Object | La valeur de la formule. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Définit la chaîne HTML qui contient des données et certains formats dans cette cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


définir le format d'affichage des nombres et des dates

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| numbertype | int | la valeur du numbertype, voir GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Obtient la copie du style de la cellule. définir le style pour la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Obtient la valeur contenue dans cette cellule.

**Remarks**

Type possible :

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne qui représente l'objet Cell actuel.

**Returns:**
java.lang.String -
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

