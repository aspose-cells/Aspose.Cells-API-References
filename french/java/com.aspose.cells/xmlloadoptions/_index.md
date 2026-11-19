---
title: "XmlLoadOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options de chargement du xml."
type: docs
url: /fr/java/com.aspose.cells/xmlloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class XmlLoadOptions extends LoadOptions
```

Représente les options de chargement du xml.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [XmlLoadOptions()](#XmlLoadOptions--) | Représente les options de chargement du fichier xml. |
| [XmlLoadOptions(int type)](#XmlLoadOptions-int-) | Représente les options de chargement du fichier xml. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [containsMultipleWorksheets()](#containsMultipleWorksheets--) | Indique si l'importation du xml se fait sous forme de plusieurs feuilles de calcul. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Obtient les options de l'ajustement automatique |
| [getCheckDataValid()](#getCheckDataValid--) | Vérifie si les données sont valides dans le fichier modèle. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getConvertNumericOrDate()](#getConvertNumericOrDate--) | Indique si la conversion de la valeur dans le fichier xml en numérique ou en date. |
| [getDateFormat()](#getDateFormat--) | Obtient le format de la valeur de date. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Obtient les paramètres de style par défaut pour l'initialisation des styles du classeur |
| [getFontConfigs()](#getFontConfigs--) | Obtient les configurations de police individuelles. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [getIgnoreRootAttributes()](#getIgnoreRootAttributes--) | Indique s'il faut ignorer les attributs de l'élément racine. |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Indique si les formes inutiles sont ignorées. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Obtient le moniteur d'interruption. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [getLanguageCode()](#getLanguageCode--) | Obtient la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [getLoadFilter()](#getLoadFilter--) | Le filtre indiquant comment charger les données. |
| [getLoadFormat()](#getLoadFormat--) | Obtient le format de chargement. |
| [getLocale()](#getLocale--) | Obtient les paramètres régionaux utilisés pour le classeur qui sera chargé. |
| [getMemorySetting()](#getMemorySetting--) | Obtient le mode mémoire pour le classeur chargé. |
| [getNumberFormat()](#getNumberFormat--) | Obtient le format de la valeur numérique. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indique si la formule est analysée lors de la lecture du fichier. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [getPassword()](#getPassword--) | Obtient le mot de passe du classeur. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [getRegion()](#getRegion--) | Obtient les paramètres régionaux utilisés pour le classeur qui sera chargé. |
| [getStandardFont()](#getStandardFont--) | Définit le nom de police standard par défaut |
| [getStandardFontSize()](#getStandardFontSize--) | Définit la taille de police standard par défaut. |
| [getStartCell()](#getStartCell--) | Obtient la cellule de départ. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hashCode()](#hashCode--) |  |
| [isXmlMap()](#isXmlMap--) | Indique s'il faut mapper le xml vers Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Définit les options de l'ajustement automatique |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Vérifie si les données sont valides dans le fichier modèle. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setContainsMultipleWorksheets(boolean value)](#setContainsMultipleWorksheets-boolean-) | Indique si l'importation du xml se fait sous forme de plusieurs feuilles de calcul. |
| [setConvertNumericOrDate(boolean value)](#setConvertNumericOrDate-boolean-) | Indique si la conversion de la valeur dans le fichier xml en numérique ou en date. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Définit le format de la valeur de date. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Définit les configurations de police individuelles. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [setIgnoreRootAttributes(boolean value)](#setIgnoreRootAttributes-boolean-) | Indique s'il faut ignorer les attributs de l'élément racine. |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Indique si les formes inutiles sont ignorées. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Définit le moniteur d’interruption. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Définit la langue de l’interface utilisateur de la version du Workbook basée sur CountryCode qui a enregistré le fichier. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Le filtre indiquant comment charger les données. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Définit les paramètres régionaux utilisés pour le Workbook qui sera chargé. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Définit le mode mémoire pour le classeur chargé. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Définit le format de la valeur numérique. |
| [setPaperSize(int type)](#setPaperSize-int-) | Définit la taille de papier d’impression par défaut à partir des paramètres de l’imprimante par défaut. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indique si la formule est analysée lors de la lecture du fichier. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Définit le mot de passe du classeur. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [setRegion(int value)](#setRegion-int-) | Définit les paramètres régionaux utilisés pour le Workbook qui sera chargé. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Définit le nom de police standard par défaut |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Définit la taille de police standard par défaut. |
| [setStartCell(String value)](#setStartCell-java.lang.String-) | Définit la cellule de départ. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [setXmlMap(boolean value)](#setXmlMap-boolean-) | Indique s'il faut mapper le xml vers Excel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XmlLoadOptions() {#XmlLoadOptions--}
```
public XmlLoadOptions()
```


Représente les options de chargement du fichier xml.

### XmlLoadOptions(int type) {#XmlLoadOptions-int-}
```
public XmlLoadOptions(int type)
```


Représente les options de chargement du fichier xml.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [LoadFormat](../../com.aspose.cells/loadformat). Le type de format de chargement. |

### containsMultipleWorksheets() {#containsMultipleWorksheets--}
```
public boolean containsMultipleWorksheets()
```


Indique si l'importation du xml se fait sous forme de plusieurs feuilles de calcul.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indique si le filtrage automatique des données est effectué lors du chargement des fichiers.

**Remarks**

Parfois, même si le filtre automatique est activé, les lignes correspondantes ne sont pas masquées dans le fichier. Fonctionne désormais uniquement pour le fichier SpreadSheetML.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Obtient les options de l'ajustement automatique

**Remarks**

Uniquement pour les fichiers xlsx, spreadsheetML maintenant.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Vérifie si les données sont valides dans le fichier modèle.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Indique s’il faut vérifier les restrictions du fichier Excel lorsque l’utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d’autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n’est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericOrDate() {#getConvertNumericOrDate--}
```
public boolean getConvertNumericOrDate()
```


Indique si la conversion de la valeur dans le fichier xml en numérique ou en date.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Obtient le format de la valeur de date.

**Returns:**
java.lang.String
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Obtient les paramètres de style par défaut pour l'initialisation des styles du classeur

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Récupère les configurations de police individuelles. Fonctionne uniquement pour le [Workbook](../../com.aspose.cells/workbook) qui utilise ces [LoadOptions](../../com.aspose.cells/loadoptions) pour le chargement.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier

**Remarks**

Uniquement pour le fichier xlsx.

**Returns:**
boolean
### getIgnoreRootAttributes() {#getIgnoreRootAttributes--}
```
public boolean getIgnoreRootAttributes()
```


Indique s'il faut ignorer les attributs de l'élément racine.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Indique si les formes inutiles sont ignorées.

**Remarks**

Fonctionne uniquement pour les fichiers xlsx, xlsb et xlsm. Il existe de nombreuses formes identiques qui se chevauchent et qui sont inutiles dans certains fichiers ; nous pouvons les ignorer lors du chargement des fichiers.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Obtient le moniteur d'interruption.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Indique s’il faut conserver les données non analysées en mémoire pour le Workbook lorsqu’il est chargé depuis un fichier modèle. La valeur par défaut est vraie.

**Remarks**

Dans les scénarios où l’utilisateur n’a besoin que de lire certains contenus du fichier modèle et n’a pas besoin d’enregistrer à nouveau le classeur, définir cette propriété à false peut améliorer les performances, notamment lorsqu’elle est utilisée conjointement avec un certain type de LoadFilter,

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Obtient la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


Le filtre indiquant comment charger les données.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Obtient le format de chargement.

Voir [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Obtient les paramètres régionaux utilisés pour le classeur qui sera chargé.

**Remarks**

Cette propriété a le même effet que [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) pour définir les paramètres régionaux.

**Returns:**
java.util.Locale
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Obtient le mode mémoire pour le classeur chargé.

Voir [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Pour plus de détails sur le mode mémoire, veuillez consulter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Obtient le format de la valeur numérique.

**Returns:**
java.lang.String
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indique si la formule est analysée lors de la lecture du fichier.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm et Xlsm car les formules dans ces fichiers sont stockées sous forme de chaîne de caractères.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Indique s’il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm, Xlsm et xlsb.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Obtient le mot de passe du classeur.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indique s'il faut conserver les espaces et les sauts de ligne qui sont remplis entre les jetons de formule lors de la lecture et de l'écriture des formules. La valeur par défaut est false.

**Remarks**

Après le chargement du classeur à partir du fichier modèle avec cette option, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) sera défini sur la même valeur que cette propriété.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Obtient les paramètres régionaux utilisés pour le classeur qui sera chargé.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Les paramètres régionaux peuvent être utilisés pour initialiser certaines fonctionnalités du classeur telles que les polices, les thèmes, etc. Pour les formats de fichiers basés sur du texte, comme CSV, HTML, ..., le paramètre régional sera également utilisé pour détecter les formats numériques et analyser les valeurs textuelles en valeurs numériques ou de date/heure pour les cellules. Ce paramètre sera conservé pour le classeur instancié ultérieurement, c’est‑à‑dire que [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) du classeur utilisera la même région que cette propriété.

**Returns:**
int
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Définit le nom de police standard par défaut

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser DefaultStyleSettings. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Définit la taille de police standard par défaut.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser DefaultStyleSettings. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
double
### getStartCell() {#getStartCell--}
```
public String getStartCell()
```


Obtient la cellule de départ.

**Remarks**

Ne fonctionne que lorsque le fichier n'est pas speadsheetML ou que le xml est mappé vers Excel.

**Returns:**
java.lang.String
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtient le rappel d'avertissement.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isXmlMap() {#isXmlMap--}
```
public boolean isXmlMap()
```


Indique s'il faut mapper le xml vers Excel. La valeur par défaut est false.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Indique si le filtrage automatique des données est effectué lors du chargement des fichiers.

**Remarks**

Parfois, même si le filtre automatique est activé, les lignes correspondantes ne sont pas masquées dans le fichier. Fonctionne désormais uniquement pour le fichier SpreadSheetML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Définit les options de l'ajustement automatique

**Remarks**

Uniquement pour les fichiers xlsx, spreadsheetML maintenant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Vérifie si les données sont valides dans le fichier modèle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Indique s’il faut vérifier les restrictions du fichier Excel lorsque l’utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d’autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n’est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setContainsMultipleWorksheets(boolean value) {#setContainsMultipleWorksheets-boolean-}
```
public void setContainsMultipleWorksheets(boolean value)
```


Indique si l'importation du xml se fait sous forme de plusieurs feuilles de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setConvertNumericOrDate(boolean value) {#setConvertNumericOrDate-boolean-}
```
public void setConvertNumericOrDate(boolean value)
```


Indique si la conversion de la valeur dans le fichier xml en numérique ou en date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


Définit le format de la valeur de date.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Définit les configurations de police individuelles. Ne fonctionne que pour le [Workbook](../../com.aspose.cells/workbook) qui utilise ces [LoadOptions](../../com.aspose.cells/loadoptions) pour le chargement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier

**Remarks**

Uniquement pour le fichier xlsx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIgnoreRootAttributes(boolean value) {#setIgnoreRootAttributes-boolean-}
```
public void setIgnoreRootAttributes(boolean value)
```


Indique s'il faut ignorer les attributs de l'élément racine.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Indique si les formes inutiles sont ignorées.

**Remarks**

Fonctionne uniquement pour les fichiers xlsx, xlsb et xlsm. Il existe de nombreuses formes identiques qui se chevauchent et qui sont inutiles dans certains fichiers ; nous pouvons les ignorer lors du chargement des fichiers.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Définit le moniteur d’interruption.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Indique s’il faut conserver les données non analysées en mémoire pour le Workbook lorsqu’il est chargé depuis un fichier modèle. La valeur par défaut est vraie.

**Remarks**

Dans les scénarios où l’utilisateur n’a besoin que de lire certains contenus du fichier modèle et n’a pas besoin d’enregistrer à nouveau le classeur, définir cette propriété à false peut améliorer les performances, notamment lorsqu’elle est utilisée conjointement avec un certain type de LoadFilter,

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Définit la langue de l’interface utilisateur de la version du Workbook basée sur CountryCode qui a enregistré le fichier.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


Le filtre indiquant comment charger les données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Définit les paramètres régionaux utilisés pour le Workbook qui sera chargé.

**Remarks**

Cette propriété a le même effet que [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) pour définir les paramètres régionaux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Locale |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Définit le mode mémoire pour le classeur chargé.

Voir [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Pour plus de détails sur le mode mémoire, veuillez consulter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Définit le format de la valeur numérique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Définit la taille de papier d’impression par défaut à partir des paramètres de l’imprimante par défaut.

**Remarks**

S'il n'existe aucun paramètre concernant la taille du papier, MS Excel utilisera le paramètre d'imprimante par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). La taille de papier par défaut. |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Indique si la formule est analysée lors de la lecture du fichier.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm et Xlsm car les formules dans ces fichiers sont stockées sous forme de chaîne de caractères.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Indique s’il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false.

**Remarks**

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm, Xlsm et xlsb.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Définit le mot de passe du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Indique s'il faut conserver les espaces et les sauts de ligne qui sont remplis entre les jetons de formule lors de la lecture et de l'écriture des formules. La valeur par défaut est false.

**Remarks**

Après le chargement du classeur à partir du fichier modèle avec cette option, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) sera défini sur la même valeur que cette propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Définit les paramètres régionaux utilisés pour le Workbook qui sera chargé.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

Les paramètres régionaux peuvent être utilisés pour initialiser certaines fonctionnalités du classeur telles que les polices, les thèmes, etc. Pour les formats de fichiers basés sur du texte, comme CSV, HTML, ..., le paramètre régional sera également utilisé pour détecter les formats numériques et analyser les valeurs textuelles en valeurs numériques ou de date/heure pour les cellules. Ce paramètre sera conservé pour le classeur instancié ultérieurement, c’est‑à‑dire que [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) du classeur utilisera la même région que cette propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Définit le nom de police standard par défaut

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser DefaultStyleSettings. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Définit la taille de police standard par défaut.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser DefaultStyleSettings. Cette propriété sera supprimée 12 mois plus tard, depuis mars 2022. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStartCell(String value) {#setStartCell-java.lang.String-}
```
public void setStartCell(String value)
```


Définit la cellule de départ.

**Remarks**

Ne fonctionne que lorsque le fichier n'est pas speadsheetML ou que le xml est mappé vers Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Définit le rappel d’avertissement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setXmlMap(boolean value) {#setXmlMap-boolean-}
```
public void setXmlMap(boolean value)
```


Indique s'il faut mapper le xml vers Excel. La valeur par défaut est false.

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

