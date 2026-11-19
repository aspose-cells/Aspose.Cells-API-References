---
title: "EbookLoadOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options lors de l'importation d'un fichier ebook."
type: docs
url: /fr/java/com.aspose.cells/ebookloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions), [com.aspose.cells.HtmlLoadOptions](../../com.aspose.cells/htmlloadoptions)
```
public class EbookLoadOptions extends HtmlLoadOptions
```

Représente les options lors de l'importation d'un fichier ebook.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [EbookLoadOptions()](#EbookLoadOptions--) | Crée une option pour charger le fichier ebook. |
| [EbookLoadOptions(int loadFormat)](#EbookLoadOptions-int-) | Crée une option de chargement du fichier ebook. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Le répertoire où les fichiers joints seront enregistrés. |
| [getAutoFilter()](#getAutoFilter--) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [getAutoFitColsAndRows()](#getAutoFitColsAndRows--) | Indique si les colonnes et lignes sont ajustées automatiquement. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Obtient les options de l'ajustement automatique |
| [getCheckDataValid()](#getCheckDataValid--) | Vérifie si les données sont valides dans le fichier modèle. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Obtient une valeur qui indique si la chaîne dans le fichier texte est convertie en données de date. |
| [getConvertFormulasData()](#getConvertFormulasData--) | si vrai, convertir la chaîne en formule lorsque la valeur de la chaîne commence par le caractère '=', la valeur par défaut est false. |
| [getConvertNumericData()](#getConvertNumericData--) | Obtient une valeur qui indique si la chaîne dans le fichier texte est convertie en données numériques. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Obtient les paramètres de style par défaut pour l'initialisation des styles du classeur |
| [getDeleteRedundantSpaces()](#getDeleteRedundantSpaces--) | Indique si les espaces redondants sont supprimés lorsque le texte renvoie des lignes en utilisant la balise `<br>`. |
| [getDetectLaTeX()](#getDetectLaTeX--) | Indique si la formule LaTeX doit être détectée dans le fichier HTML. |
| [getEncoding()](#getEncoding--) | Obtient le codage par défaut. |
| [getFontConfigs()](#getFontConfigs--) | Obtient les configurations de police individuelles. |
| [getHyperlinkLoadMode()](#getHyperlinkLoadMode--) | Spécifie comment les hyperliens sont chargés lors du chargement du HTML. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Indique si les formes inutiles sont ignorées. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Obtient le moniteur d'interruption. |
| [getKeepPrecision()](#getKeepPrecision--) | Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [getLanguageCode()](#getLanguageCode--) | Obtient la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [getLoadFilter()](#getLoadFilter--) | Le filtre indiquant comment charger les données. |
| [getLoadFormat()](#getLoadFormat--) | Obtient le format de chargement. |
| [getLoadFormulas()](#getLoadFormulas--) | Indique s'il faut importer les formules si le fichier HTML original contient des formules. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure. |
| [getLocale()](#getLocale--) | Obtient les paramètres régionaux utilisés pour le classeur qui sera chargé. |
| [getMemorySetting()](#getMemorySetting--) | Obtient le mode mémoire pour le classeur chargé. |
| [getParagrahLayoutMode()](#getParagrahLayoutMode--) | Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. |
| [getParagraphLayoutMode()](#getParagraphLayoutMode--) | Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indique si la formule est analysée lors de la lecture du fichier. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [getPassword()](#getPassword--) | Obtient le mot de passe du classeur. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [getProgId()](#getProgId--) | Obtient l'identifiant du programme qui crée le fichier. |
| [getRegion()](#getRegion--) | Obtient les paramètres régionaux utilisés pour le classeur qui sera chargé. |
| [getStandardFont()](#getStandardFont--) | Définit le nom de police standard par défaut |
| [getStandardFontSize()](#getStandardFontSize--) | Définit la taille de police standard par défaut. |
| [getStreamProvider()](#getStreamProvider--) | Obtient le StreamProviderImportHtmlFile pour l'importation d'objets. |
| [getSupportDivTag()](#getSupportDivTag--) | Indique si la mise en page de la balise `<div>` est prise en charge lorsque le fichier HTML la contient. |
| [getTableLoadOptions()](#getTableLoadOptions--) | Obtenez l'instance de HtmlTableLoadOptionCollection |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [hasFormula()](#hasFormula--) | Indique si le texte est une formule s'il commence par "=". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Le répertoire où les fichiers joints seront enregistrés. |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indique si le filtrage automatique des données est effectué lors du chargement des fichiers. |
| [setAutoFitColsAndRows(boolean value)](#setAutoFitColsAndRows-boolean-) | Indique si les colonnes et lignes sont ajustées automatiquement. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Définit les options de l'ajustement automatique |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Vérifie si les données sont valides dans le fichier modèle. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date. |
| [setConvertFormulasData(boolean value)](#setConvertFormulasData-boolean-) | si vrai, convertir la chaîne en formule lorsque la valeur de la chaîne commence par le caractère '=', la valeur par défaut est false. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques. |
| [setDeleteRedundantSpaces(boolean value)](#setDeleteRedundantSpaces-boolean-) | Indique si les espaces redondants sont supprimés lorsque le texte renvoie des lignes en utilisant la balise `<br>`. |
| [setDetectLaTeX(boolean value)](#setDetectLaTeX-boolean-) | Indique si la formule LaTeX doit être détectée dans le fichier HTML. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Définit le codage par défaut. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Définit les configurations de police individuelles. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indique si le texte est une formule s'il commence par "=". |
| [setHyperlinkLoadMode(int value)](#setHyperlinkLoadMode-int-) | Spécifie comment les hyperliens sont chargés lors du chargement du HTML. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Indique si les formes inutiles sont ignorées. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Définit le moniteur d’interruption. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier modèle. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Définit la langue de l’interface utilisateur de la version du Workbook basée sur CountryCode qui a enregistré le fichier. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Le filtre indiquant comment charger les données. |
| [setLoadFormulas(boolean value)](#setLoadFormulas-boolean-) | Indique s'il faut importer les formules si le fichier HTML original contient des formules. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Définit les paramètres régionaux utilisés pour le Workbook qui sera chargé. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Définit le mode mémoire pour le classeur chargé. |
| [setPaperSize(int type)](#setPaperSize-int-) | Définit la taille de papier d’impression par défaut à partir des paramètres de l’imprimante par défaut. |
| [setParagrahLayoutMode(int value)](#setParagrahLayoutMode-int-) | Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. |
| [setParagraphLayoutMode(int value)](#setParagraphLayoutMode-int-) | Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indique si la formule est analysée lors de la lecture du fichier. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Définit le mot de passe du classeur. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indique s'il faut préserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. |
| [setRegion(int value)](#setRegion-int-) | Définit les paramètres régionaux utilisés pour le Workbook qui sera chargé. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Définit le nom de police standard par défaut |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Définit la taille de police standard par défaut. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Définit le StreamProviderImportHtmlFile pour l'importation d'objets. |
| [setSupportDivTag(boolean value)](#setSupportDivTag-boolean-) | Indique si la mise en page de la balise `<div>` est prise en charge lorsque le fichier HTML la contient. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookLoadOptions() {#EbookLoadOptions--}
```
public EbookLoadOptions()
```


Crée une option pour charger le fichier ebook.

### EbookLoadOptions(int loadFormat) {#EbookLoadOptions-int-}
```
public EbookLoadOptions(int loadFormat)
```


Crée une option de chargement du fichier ebook.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Le format de chargement |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Le répertoire où les fichiers joints seront enregistrés.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété HtmlLoadOptions.StreamProvider. Cette propriété sera supprimée 12 mois après, depuis décembre 2014. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indique si le filtrage automatique des données est effectué lors du chargement des fichiers.

**Remarks**

Parfois, même si le filtre automatique est activé, les lignes correspondantes ne sont pas masquées dans le fichier. Fonctionne désormais uniquement pour le fichier SpreadSheetML.

**Returns:**
boolean
### getAutoFitColsAndRows() {#getAutoFitColsAndRows--}
```
public boolean getAutoFitColsAndRows()
```


Indique si les colonnes et les lignes sont ajustées automatiquement. La valeur par défaut est false.

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
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Obtient une valeur qui indique si la chaîne du fichier texte est convertie en données de date. La valeur par défaut est true.

**Returns:**
boolean
### getConvertFormulasData() {#getConvertFormulasData--}
```
public boolean getConvertFormulasData()
```


si vrai, convertir la chaîne en formule lorsque la valeur de la chaîne commence par le caractère '=', la valeur par défaut est false.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété HtmlLoadOptions.HasFormula. Cette propriété sera supprimée 12 mois après, depuis mars 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Obtient une valeur qui indique si la chaîne du fichier texte est convertie en données numériques. La valeur par défaut est true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Obtient les paramètres de style par défaut pour l'initialisation des styles du classeur

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDeleteRedundantSpaces() {#getDeleteRedundantSpaces--}
```
public boolean getDeleteRedundantSpaces()
```


Indique s'il faut supprimer les espaces redondants lorsque le texte passe à la ligne en utilisant la balise `<br>`. La valeur par défaut est false.

**Returns:**
boolean
### getDetectLaTeX() {#getDetectLaTeX--}
```
public boolean getDetectLaTeX()
```


Indique s'il faut détecter les formules LaTeX dans le fichier HTML. La valeur par défaut est false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Obtient le codage par défaut. S'applique uniquement aux fichiers csv.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Récupère les configurations de police individuelles. Fonctionne uniquement pour le [Workbook](../../com.aspose.cells/workbook) qui utilise ces [LoadOptions](../../com.aspose.cells/loadoptions) pour le chargement.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHyperlinkLoadMode() {#getHyperlinkLoadMode--}
```
public int getHyperlinkLoadMode()
```


Spécifie comment les hyperliens sont chargés lors du chargement du HTML.

Voir [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier

**Remarks**

Uniquement pour le fichier xlsx.

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
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15.

**Returns:**
boolean
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
### getLoadFormulas() {#getLoadFormulas--}
```
public boolean getLoadFormulas()
```


Indique s'il faut importer les formules si le fichier HTML original contient des formules.

**Returns:**
boolean
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure.

Voir [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

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
### getParagrahLayoutMode() {#getParagrahLayoutMode--}
```
public int getParagrahLayoutMode()
```


Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. La valeur par défaut est [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Voir [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlLoadOptions.ParagraphLayoutMode. Cette méthode sera supprimée 12 mois plus tard, à partir de juillet 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getParagraphLayoutMode() {#getParagraphLayoutMode--}
```
public int getParagraphLayoutMode()
```


Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. La valeur par défaut est [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Voir [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Returns:**
int
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
### getProgId() {#getProgId--}
```
public String getProgId()
```


Obtient l’identifiant du programme de création du fichier. Uniquement pour les fichiers MHT.

**Returns:**
java.lang.String
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
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Obtient le StreamProviderImportHtmlFile pour l'importation d'objets.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getSupportDivTag() {#getSupportDivTag--}
```
public boolean getSupportDivTag()
```


Indique si la prise en charge de la mise en page de la balise `<div>` est activée lorsque le fichier HTML la contient. La valeur par défaut est false.

**Returns:**
boolean
### getTableLoadOptions() {#getTableLoadOptions--}
```
public HtmlTableLoadOptionCollection getTableLoadOptions()
```


Obtenez l'instance de HtmlTableLoadOptionCollection

**Returns:**
[HtmlTableLoadOptionCollection](../../com.aspose.cells/htmltableloadoptioncollection)
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtient le rappel d'avertissement.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Indique si le texte est une formule s'il commence par "=".

**Returns:**
boolean
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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Le répertoire où les fichiers joints seront enregistrés.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété HtmlLoadOptions.StreamProvider. Cette propriété sera supprimée 12 mois après, depuis décembre 2014. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setAutoFitColsAndRows(boolean value) {#setAutoFitColsAndRows-boolean-}
```
public void setAutoFitColsAndRows(boolean value)
```


Indique si les colonnes et les lignes sont ajustées automatiquement. La valeur par défaut est false.

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

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Définit une valeur indiquant si la chaîne du fichier texte est convertie en données de type date. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setConvertFormulasData(boolean value) {#setConvertFormulasData-boolean-}
```
public void setConvertFormulasData(boolean value)
```


si vrai, convertir la chaîne en formule lorsque la valeur de la chaîne commence par le caractère '=', la valeur par défaut est false.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété HtmlLoadOptions.HasFormula. Cette propriété sera supprimée 12 mois après, depuis mars 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Définit une valeur indiquant si la chaîne du fichier texte est convertie en données numériques. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDeleteRedundantSpaces(boolean value) {#setDeleteRedundantSpaces-boolean-}
```
public void setDeleteRedundantSpaces(boolean value)
```


Indique s'il faut supprimer les espaces redondants lorsque le texte passe à la ligne en utilisant la balise `<br>`. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDetectLaTeX(boolean value) {#setDetectLaTeX-boolean-}
```
public void setDetectLaTeX(boolean value)
```


Indique s'il faut détecter les formules LaTeX dans le fichier HTML. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Définit l’encodage par défaut. S’applique uniquement aux fichiers csv.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Définit les configurations de police individuelles. Ne fonctionne que pour le [Workbook](../../com.aspose.cells/workbook) qui utilise ces [LoadOptions](../../com.aspose.cells/loadoptions) pour le chargement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Indique si le texte est une formule s'il commence par "=".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHyperlinkLoadMode(int value) {#setHyperlinkLoadMode-int-}
```
public void setHyperlinkLoadMode(int value)
```


Spécifie comment les hyperliens sont chargés lors du chargement du HTML.

Voir [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setLoadFormulas(boolean value) {#setLoadFormulas-boolean-}
```
public void setLoadFormulas(boolean value)
```


Indique s'il faut importer les formules si le fichier HTML original contient des formules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure.

Voir [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setParagrahLayoutMode(int value) {#setParagrahLayoutMode-int-}
```
public void setParagrahLayoutMode(int value)
```


Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. La valeur par défaut est [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Voir [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlLoadOptions.ParagraphLayoutMode. Cette méthode sera supprimée 12 mois plus tard, à partir de juillet 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setParagraphLayoutMode(int value) {#setParagraphLayoutMode-int-}
```
public void setParagraphLayoutMode(int value)
```


Spécifie comment les éléments HTML <p> sont rendus lors du chargement du HTML. La valeur par défaut est [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL).

Voir [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Définit le StreamProviderImportHtmlFile pour l'importation d'objets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setSupportDivTag(boolean value) {#setSupportDivTag-boolean-}
```
public void setSupportDivTag(boolean value)
```


Indique si la prise en charge de la mise en page de la balise `<div>` est activée lorsque le fichier HTML la contient. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Définit le rappel d’avertissement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

