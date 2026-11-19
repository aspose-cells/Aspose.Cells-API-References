---
title: "WorksheetDesign"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Hérité de WebWorksheet."
type: docs
url: /fr/java/com.aspose.gridweb/worksheetdesign/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control), [com.aspose.gridweb.WebWorksheet](../../com.aspose.gridweb/webworksheet)
```
public class WorksheetDesign extends WebWorksheet
```

Hérité de WebWorksheet. Utilisé uniquement en mode conception.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WorksheetDesign()](#WorksheetDesign--) | Constructeur par défaut. |
| [WorksheetDesign(MainWeb mw, GridWorksheet gwk)](#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | le constructeur avec MainWeb et GridWorksheet |
## Méthodes

| Méthode | Description |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Ajuste automatiquement la largeur de la colonne. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Ajuste automatiquement la largeur de la colonne. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Annule et supprime la nouvelle ligne liée ajoutée. |
| [commitNewBindRow()](#commitNewBindRow--) | Valide la nouvelle ligne liée ajoutée et l'ajoute à la source de données. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Copie depuis un autre objet de feuille de calcul. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | Après avoir défini une source de données pour la feuille de calcul, appelez cette méthode pour générer automatiquement les colonnes liées. |
| [createNewBindRow()](#createNewBindRow--) | Crée une nouvelle ligne liée et la lie à la source de données. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Crée un sous-total dans la feuille. |
| [dataBind()](#dataBind--) | Liez la feuille à la DataSource. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Supprime une ligne liée. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Fige les volets à la cellule spécifiée dans la feuille de calcul. |
| [getBindStartColumn()](#getBindStartColumn--) | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [getBindStartRow()](#getBindStartRow--) | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [getBindingSource()](#getBindingSource--) | L'objet source de données réellement lié à l'exécution. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Obtient le nombre de lignes liées en mode liaison de données. |
| [getDataMember()](#getDataMember--) | Obtient le DataMember de la source de données multi-membres. |
| [getDataSource()](#getDataSource--) | Obtient la DataSource. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | En mode liaison de données, indique s'il faut créer des légendes d'en-tête de colonne liées dans la feuille. |
| [getIndex()](#getIndex--) | Obtient l'index de lui-même dans les feuilles de calcul. |
| [getName()](#getName--) | Obtient le nom de la feuille. |
| [getUniqueID()](#getUniqueID--) | Obtient l'UniqueID dans le Contrôle |
| [getValidations()](#getValidations--) | Obtient la collection des paramètres de validation des données dans la feuille de calcul. |
| [getVisible()](#getVisible--) | Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Regroupe les lignes. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Regroupe les lignes. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Obtient si la feuille de calcul est protégée. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Rend toutes les cellules modifiables. Ceci est un attribut étendu. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Rend toutes les cellules en lecture seule. Ceci est un attribut étendu, notez que cet attribut ne peut pas être conservé dans la cellule réelle ; si vous souhaitez conserver la protection, veuillez utiliser setProtect. |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Obtient le nombre de lignes liées en mode liaison de données. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Définit le DataMember à partir du DataSource multi-membres. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | Définit le DataSource. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Rend une plage de cellules modifiable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendre toutes les cellules en lecture seule en appelant la méthode SetAllCellsReadonly. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | En mode liaison de données, indique s'il faut créer des légendes d'en-tête de colonne liées dans la feuille. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la feuille. |
| [setProtected(boolean value)](#setProtected-boolean-) | Définit si la feuille de calcul est protégée. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Rend une plage de cellules en lecture seule. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Commencez par rendre toutes les cellules modifiables en appelant la méthode SetAllCellsEditable. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Déverrouille les volets dans la feuille de calcul. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Dégroupe les lignes. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorksheetDesign() {#WorksheetDesign--}
```
public WorksheetDesign()
```


Constructeur par défaut.

### WorksheetDesign(MainWeb mw, GridWorksheet gwk) {#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WorksheetDesign(MainWeb mw, GridWorksheet gwk)
```


le constructeur avec MainWeb et GridWorksheet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Ajuste automatiquement la largeur de la colonne.

**Remarks**

AutoFitColumn est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | Indice de colonne. |

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


Ajuste automatiquement la largeur de la colonne. Cette méthode ajuste automatiquement une colonne en fonction du contenu d'une plage de cellules de la colonne, de startRow à endRow. AutoFitColumn est une fonction imprécise.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | indice de colonne, basé sur zéro |
| startRow | int | indice de ligne de départ, basé sur zéro |
| endRow | int | indice de ligne de fin, basé sur zéro |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


Annule et supprime la nouvelle ligne liée ajoutée.

**Returns:**
int - L'indice de ligne. S'il n'y a aucune nouvelle ligne liée créée, renvoie -1.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


Valide la nouvelle ligne liée ajoutée et l'ajoute à la source de données.

**Returns:**
int - L'indice de ligne de la nouvelle ligne. Si aucune ligne n'est créée, renvoie -1.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


Copie depuis un autre objet de feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | L'autre feuille. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


Après avoir défini une source de données pour la feuille de calcul, appelez cette méthode pour générer automatiquement les colonnes liées.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


Crée une nouvelle ligne liée et la lie à la source de données.

**Returns:**
int - L'indice de ligne de la nouvelle ligne. Si aucune ligne n'est créée, renvoie -1.
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Crée un sous-total dans la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnNameRowIndex | int | L'index de ligne de la ligne de nom de colonne. |
| dataRows | int | Le nombre de lignes de données. |
| groupByColumnIndex | int | L'index de colonne de la colonne à regrouper. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Le type de fonction de sous-total. |
| subtotalColumnIndexList | int[] | Les index de colonnes à sous-totaliser. |
| functionLabel | java.lang.String | L'étiquette de la fonction de sous-total. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Le style de la ligne du total général. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Le style de la ligne de sous-total. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Le type numérique des cellules de résultat du sous-total. |
| customString | java.lang.String | La chaîne de format personnalisée des cellules de résultat du sous-total. Peut être nulle. |

### dataBind() {#dataBind--}
```
public void dataBind()
```


Liez la feuille à la DataSource.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


Supprime une ligne liée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowNum | int | L'index de ligne. |

**Returns:**
int - L'indice de ligne supprimée. Si aucune ligne liée n'est supprimée, renvoie -1.
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
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Fige les volets à la cellule spécifiée dans la feuille de calcul.

**Remarks**

L'index de ligne et l'index de colonne ne peuvent pas tous les deux être zéro. Le nombre de lignes et le nombre de colonnes ne peuvent pas non plus être tous les deux zéro.

Les deux premiers paramètres spécifient la position gelée et les deux derniers paramètres spécifient la zone gelée dans le volet supérieur gauche.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne. |
| colonne | int | Indice de colonne. |
| freezedRows | int | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | int | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


L'objet datasource réellement lié à l'exécution. C'est un objet DataView lorsque la propriété DataSource est un objet DataSet, DataTable ou DataView.

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


Obtient le nombre de lignes liées en mode liaison de données.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


Obtient le DataMember à partir du DataSource multi-membres. Généralement, il représente un objet DataTable d'un DataSet.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


Obtient le DataSource. Généralement, c'est un objet DataSet.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


En mode liaison de données, indique s'il faut créer des légendes d'en-tête de colonne liées dans la feuille.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'index de lui-même dans les feuilles de calcul.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la feuille.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Obtient l'UniqueID dans le Contrôle

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Obtient la collection des paramètres de validation des données dans la feuille de calcul.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle.

**Returns:**
boolean
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Regroupe les lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à regrouper. |
| lastIndex | int | Le dernier indice de ligne à regrouper. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Regroupe les lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à regrouper. |
| lastIndex | int | Le dernier indice de ligne à regrouper. |
| isHidden | boolean | Spécifie si les lignes regroupées sont masquées. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Obtient si la feuille de calcul est protégée. Lorsqu'une feuille de calcul est protégée, toutes les cellules ne peuvent pas être modifiées sauf la cellule dont la propriété IsLocked est false.

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




### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Rend toutes les cellules modifiables. Ceci est un attribut étendu.

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Rend toutes les cellules en lecture seule. Ceci est un attribut étendu, notez que cet attribut ne peut pas être conservé dans la cellule réelle ; si vous souhaitez conserver la protection, veuillez utiliser setProtect.

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


En mode liaison de données, BindStartRow et BindStartColumn indiquent la position de la grille à lier à la source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


Obtient le nombre de lignes liées en mode liaison de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


Définit le DataMember à partir du DataSource multi-membres. Généralement, il représente un objet DataTable d'un DataSet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


Définit le DataSource. Généralement, c'est un objet DataSet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Rend une plage de cellules modifiable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendre toutes les cellules en lecture seule en appelant la méthode SetAllCellsReadonly. puis appelez cette méthode pour spécifier la plage de cellules qui doit être modifiable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ de la plage. |
| startColumn | int | La colonne de départ de la plage. |
| lignes | int | Le nombre de lignes. |
| colonnes | int | Le nombre de colonnes. |

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


En mode liaison de données, indique s'il faut créer des légendes d'en-tête de colonne liées dans la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


Définit si la feuille de calcul est protégée. Lorsqu'une feuille de calcul est protégée, toutes les cellules ne peuvent pas être modifiées sauf la cellule dont la propriété IsLocked est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Rend une plage de cellules en lecture seule. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Commencez par rendre toutes les cellules modifiables en appelant la méthode SetAllCellsEditable. puis appelez cette méthode pour spécifier la plage de cellules qui doit être en lecture seule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | int | La ligne de départ de la plage. |
| startColumn | int | La colonne de départ de la plage. |
| lignes | int | Le nombre de lignes. |
| colonnes | int | Le nombre de colonnes. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indique si le nom de cette feuille est affiché dans les onglets de feuilles du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


Déverrouille les volets dans la feuille de calcul.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Dégroupe les lignes.

**Remarks**

Supprime uniquement les informations du groupe externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | int | Le premier indice de ligne à dégrouper. |
| lastIndex | int | Le dernier indice de ligne à dégrouper. |

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

