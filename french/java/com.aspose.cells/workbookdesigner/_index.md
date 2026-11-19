---
title: "WorkbookDesigner"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une feuille de calcul de concepteur."
type: docs
url: /fr/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

Encapsule l'objet qui représente une feuille de calcul de concepteur.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | Initialise une nouvelle instance de la classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | Initialise une nouvelle instance de la classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | Efface toutes les sources de données. |
| [containsVariables()](#containsVariables--) | Indique si la première feuille de calcul contient des variables personnalisées. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | Indique si les formules doivent être calculées. |
| [getCallBack()](#getCallBack--) | Obtient l'interface de rappel du traitement du smartmarker. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | Indique si l'en-tête/pied de page contient des marqueurs intelligents et doit être traité ensemble. |
| [getLineByLine()](#getLineByLine--) | Indique si le traitement du marqueur intelligent se fait ligne par ligne. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | Indique si les formules répétées avec une ligne de sous-total sont présentes. |
| [getSmartMarkers()](#getSmartMarkers--) | Renvoie une collection de marqueurs intelligents dans une feuille de calcul. |
| [getSortDataSource()](#getSortDataSource--) | Indique si la source de données est triée. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | Si TRUE, Null sera inséré si la valeur est "" ; |
| [getUpdateReference()](#getUpdateReference--) | Indique si les références dans d’autres feuilles de calcul seront mises à jour. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | Obtient le nom de la feuille de calcul contenant le marqueur intelligent de variables. |
| [getWorkbook()](#getWorkbook--) | Obtient l'objet [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | Traite les marqueurs intelligents et remplit les valeurs de la source de données. |
| [process(boolean isPreserved)](#process-boolean-) | Traite les marqueurs intelligents et remplit les valeurs de la source de données. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | Traite les marqueurs intelligents et remplit les valeurs de la source de données. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | Traite les marqueurs intelligents et remplit les valeurs de la source de données. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indique si les formules doivent être calculées. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | Définit l'interface de rappel du traitement du smartmarker. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | Indique si la première feuille de calcul contient des variables personnalisées. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | Définit la source de données d'un objet [ICellsDataTable](../../com.aspose.cells/icellsdatatable). |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | Définit la liaison de données à une variable. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | Définir la source de données. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | Définir la source de données. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | Définir la source de données. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | Indique si l'en-tête/pied de page contient des marqueurs intelligents et doit être traité ensemble. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | Définir la valeur de chaîne JSON comme source de données des marqueurs intelligents. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | Indique si le traitement du marqueur intelligent se fait ligne par ligne. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | Indique si les formules répétées avec une ligne de sous-total sont présentes. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | Indique si la source de données est triée. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | Si TRUE, Null sera inséré si la valeur est "" ; |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indique si les références dans d’autres feuilles de calcul seront mises à jour. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | Définit le nom de la feuille de calcul contenant le marqueur intelligent de variables. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | Définit l'objet [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


Initialise une nouvelle instance de la classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


Initialise une nouvelle instance de la classe [WorkbookDesigner](../../com.aspose.cells/workbookdesigner).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Le fichier de classeur modèle. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


Efface toutes les sources de données.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


Indique si la première feuille de calcul contient des variables personnalisées.

**Remarks**

NOTE: Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété WorkbookDesigner.VariablesWorksheetName. Cette propriété sera supprimée dans 3 mois, à compter de septembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
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
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indique si les formules doivent être calculées.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


Obtient l'interface de rappel du traitement du smartmarker.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


Indique si l'en-tête/pied de page contient des marqueurs intelligents et doit être traité ensemble.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


Indique si le traitement du marqueur intelligent se fait ligne par ligne.

**Remarks**

NOTE: Cette classe est maintenant obsolète. Veuillez plutôt utiliser les marqueurs intelligents de plage. Cette propriété sera supprimée dans 12 mois, à compter de juillet 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


Indique si les formules répétées avec une ligne de sous-total sont présentes.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


Renvoie une collection de marqueurs intelligents dans une feuille de calcul.

**Remarks**

Un tableau de chaînes est créé à chaque appel. Le tableau est trié et les valeurs dupliquées sont supprimées.

**Returns:**
java.lang.String[] - Une collection de marqueurs intelligents
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


Indique si la source de données est triée.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. Elle sera supprimée dans 12 mois, à compter d’octobre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer. La source de données Json sera triée si le smart marker contient des paramètres d’ordre croissant et décroissant.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


Si TRUE, Null sera inséré si la valeur est "" ;

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Indique si les références dans d’autres feuilles de calcul seront mises à jour.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


Obtient le nom de la feuille de calcul contenant le marqueur intelligent de variables.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Obtient l'objet [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
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




### process() {#process--}
```
public void process()
```


Traite les marqueurs intelligents et remplit les valeurs de la source de données.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


Traite les marqueurs intelligents et remplit les valeurs de la source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| isPreserved | boolean | Vrai si le smart marker non reconnu est préservé. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


Traite les marqueurs intelligents et remplit les valeurs de la source de données.

**Remarks**

NOTE: Cette classe est maintenant obsolète. Veuillez plutôt utiliser les marqueurs intelligents Range. Cette propriété sera supprimée dans 12 mois, à compter de juillet 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage à traiter |
| isPreserved | boolean | Vrai si le smart marker non reconnu est préservé. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


Traite les marqueurs intelligents et remplit les valeurs de la source de données.

**Remarks**

Cette méthode fonctionne au niveau de la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Indice de la feuille de calcul. |
| isPreserved | boolean | Vrai si le smart marker non reconnu est préservé. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indique si les formules doivent être calculées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


Définit l'interface de rappel du traitement du smartmarker.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


Indique si la première feuille de calcul contient des variables personnalisées.

**Remarks**

NOTE: Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété WorkbookDesigner.VariablesWorksheetName. Cette propriété sera supprimée dans 3 mois, à compter de septembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


Définit la source de données d'un objet [ICellsDataTable](../../com.aspose.cells/icellsdatatable).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dataSource | java.lang.String | Le nom de la source de données. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | Table de données. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


Définit la liaison de données à une variable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| variable | java.lang.String | Nom de variable créé à l'aide du marqueur intelligent. |
| données | java.lang.Object | Données source. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


Définir la source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dataSource | java.lang.String | Le nom de la source de données. |
| rs | java.sql.ResultSet | Le jeu de résultats. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


Définir la source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dataSource | java.lang.String | Le nom de la source de données. |
| rs | java.sql.ResultSet | Le jeu de résultats. |
| rowCount | int | Le nombre de données du jeu de résultats donné. Il doit être le nombre exact de lignes ou -1; si le jeu de résultats est uniquement en avant, l'utilisateur doit fournir le nombre exact de lignes ici, sinon le marqueur intelligent peut ne pas être traité correctement lorsque le "noadd" du marqueur intelligent n'est pas défini. |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


Définir la source de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rs | java.sql.ResultSet | Le jeu de résultats. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


Indique si l'en-tête/pied de page contient des marqueurs intelligents et doit être traité ensemble.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


Définir la valeur de chaîne JSON comme source de données des marqueurs intelligents.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la table. Si la valeur du JSON représente un objet, elle peut être nulle. |
| json | java.lang.String | La valeur de la chaîne Json. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


Indique si le traitement du marqueur intelligent se fait ligne par ligne.

**Remarks**

NOTE: Cette classe est maintenant obsolète. Veuillez plutôt utiliser les marqueurs intelligents de plage. Cette propriété sera supprimée dans 12 mois, à compter de juillet 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


Indique si les formules répétées avec une ligne de sous-total sont présentes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


Indique si la source de données est triée.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. Elle sera supprimée dans 12 mois, à compter d’octobre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer. La source de données Json sera triée si le smart marker contient des paramètres d’ordre croissant et décroissant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


Si TRUE, Null sera inséré si la valeur est "" ;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Indique si les références dans d’autres feuilles de calcul seront mises à jour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


Définit le nom de la feuille de calcul contenant le marqueur intelligent de variables.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


Définit l'objet [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

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

