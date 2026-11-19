---
title: "WorkbookSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente tous les paramètres du classeur."
type: docs
url: /fr/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Représente tous les paramètres du classeur.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [dispose()](#dispose--) | Libère les ressources. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Obtient l'auteur du fichier. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur. |
| [getAutoRecover()](#getAutoRecover--) | Indique si le fichier est marqué pour la récupération automatique. |
| [getBuildVersion()](#getBuildVersion--) | Spécifie la version publique incrémentale de l'application. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Indique s'il faut vérifier la compatibilité avec les versions antérieures lors de l'enregistrement du classeur. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indique s'il faut vérifier le format numérique personnalisé lors du réglage de Style.Custom. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Spécifie la version OOXML du document de sortie. |
| [getCrashSave()](#getCrashSave--) | indique si l'application a enregistré le fichier du classeur après un plantage. |
| [getDataExtractLoad()](#getDataExtractLoad--) | indique si l'application a ouvert le classeur pour la récupération des données. |
| [getDate1904()](#getDate1904--) | Obtient une valeur qui représente si le classeur utilise le système de dates 1904. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Obtient la résolution par défaut de l'image. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Obtient les paramètres des valeurs par défaut des propriétés liées au style pour ce classeur. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Indique s'il faut abandonner les données d'image en cours d'édition. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Indique si et comment afficher les objets dans le classeur. |
| [getEnableMacros()](#getEnableMacros--) | Activer les macros; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | Obtient le premier onglet de feuille de calcul visible. |
| [getFormulaSettings()](#getFormulaSettings--) | Obtient les paramètres des fonctionnalités liées aux formules. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Obtient les paramètres de mondialisation. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | Obtient si la liste des champs du tableau croisé dynamique est masquée. |
| [getLanguageCode()](#getLanguageCode--) | Obtient la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier. |
| [getLocale()](#getLocale--) | Obtient la locale utilisée par ce classeur. |
| [getMaxColumn()](#getMaxColumn--) | Obtient l'index maximal de colonne, basé sur zéro. |
| [getMaxRow()](#getMaxRow--) | Obtient l'index maximal de ligne, basé sur zéro. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Obtient le numéro maximal de ligne de la formule partagée. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Obtient la limitation des éléments uniques par champ |
| [getMemorySetting()](#getMemorySetting--) | Obtient les options d'utilisation de la mémoire. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Obtient le séparateur décimal pour le formatage/l'analyse des valeurs numériques. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Obtient le caractère qui sépare les groupes de chiffres à gauche du séparateur décimal dans les valeurs numériques. |
| [getPaperSize()](#getPaperSize--) | Obtient la taille de papier d'impression par défaut. |
| [getPassword()](#getPassword--) | Représente le mot de passe de chiffrement du fichier Workbook. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Indique si les propriétés des points de données et les étiquettes de données dans tous les graphiques de ce Workbook suivent leur référence. |
| [getProtectionType()](#getProtectionType--) | Obtient le type de protection du Workbook. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Indique si la définition de la propriété [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) lors de la saisie de la valeur chaîne (qui commence par une apostrophe) dans la cellule |
| [getRegion()](#getRegion--) | Obtient les paramètres régionaux du Workbook. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | Vrai si les informations personnelles peuvent être supprimées du Workbook spécifié. |
| [getRepairLoad()](#getRepairLoad--) | Indique si l'application a ouvert le Workbook en dernier en mode sécurisé ou de réparation. |
| [getResourceProvider()](#getResourceProvider--) | Obtient le fournisseur de flux pour la ressource externe, comme le chargement des données d'image pour une image de type "LinkToFile". |
| [getShapeDisplayType()](#getShapeDisplayType--) | Obtient la façon dont l'application affiche les formes dans ce Workbook |
| [getShared()](#getShared--) | Obtient une valeur indiquant si le Workbook est partagé. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Largeur de la barre d'onglets de la feuille de calcul (en 1/1000 de la largeur de la fenêtre). |
| [getShowTabs()](#getShowTabs--) | Obtient une valeur indiquant si les onglets du Workbook sont affichés. |
| [getSignificantDigits()](#getSignificantDigits--) | Obtient le nombre de chiffres significatifs. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Obtient le type de chiffres significatifs pour la sortie des valeurs numériques dans ce Workbook. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Obtient les options de la balise intelligente. |
| [getStreamProvider()](#getStreamProvider--) | Obtient le fournisseur de flux pour la ressource externe. |
| [getThemeFont(int type)](#getThemeFont-int-) | Obtient le nom de police du thème par défaut. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Indique si la bordure des cellules adjacentes est mise à jour. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Obtient la façon dont les liens externes sont mis à jour lorsque le Workbook est ouvert. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [getWindowHeight()](#getWindowHeight--) | La hauteur de la fenêtre, en points. |
| [getWindowHeightCM()](#getWindowHeightCM--) | La hauteur de la fenêtre, en centimètres. |
| [getWindowHeightInch()](#getWindowHeightInch--) | La hauteur de la fenêtre, en unité de pouce. |
| [getWindowLeft()](#getWindowLeft--) | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre, en unité de point. |
| [getWindowLeftCM()](#getWindowLeftCM--) | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. |
| [getWindowLeftInch()](#getWindowLeftInch--) | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. |
| [getWindowTop()](#getWindowTop--) | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de point. |
| [getWindowTopCM()](#getWindowTopCM--) | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de centimètre. |
| [getWindowTopInch()](#getWindowTopInch--) | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de pouce. |
| [getWindowWidth()](#getWindowWidth--) | La largeur de la fenêtre, en unité de point. |
| [getWindowWidthCM()](#getWindowWidthCM--) | La largeur de la fenêtre, en unité de centimètre. |
| [getWindowWidthInch()](#getWindowWidthInch--) | La largeur de la fenêtre, en unité de pouce. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Indique si la compatibilité avec WPS doit être activée. |
| [getWriteProtection()](#getWriteProtection--) | Fournit l'accès aux options de protection en écriture du classeur. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Indique si le classeur doit être chiffré avec le mot de passe par défaut lorsque la structure et les fenêtres du classeur sont verrouillés. |
| [isEncrypted()](#isEncrypted--) | Obtient une valeur qui indique si un mot de passe est requis pour ouvrir ce classeur. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Obtient une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale. |
| [isHidden()](#isHidden--) | Indique si ce classeur est masqué. |
| [isMinimized()](#isMinimized--) | Représente si la feuille de calcul générée sera ouverte minimisée. |
| [isProtected()](#isProtected--) | Obtient une valeur qui indique si la structure ou la fenêtre du classeur est protégée. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Obtient une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Définit l'auteur du fichier. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Indique si le fichier est marqué pour la récupération automatique. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Spécifie la version publique incrémentale de l'application. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Indique s'il faut vérifier la compatibilité avec les versions antérieures lors de l'enregistrement du classeur. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indique s'il faut vérifier le format numérique personnalisé lors du réglage de Style.Custom. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setCompliance(int value)](#setCompliance-int-) | Spécifie la version OOXML du document de sortie. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | indique si l'application a enregistré le fichier du classeur après un plantage. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | indique si l'application a ouvert le classeur pour la récupération des données. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Définit une valeur qui représente si le classeur utilise le système de date 1904. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Indique si le classeur doit être chiffré avec le mot de passe par défaut lorsque la structure et les fenêtres du classeur sont verrouillés. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Définit la résolution par défaut de l'image. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Indique s'il faut abandonner les données d'image en cours d'édition. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Indique si et comment afficher les objets dans le classeur. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Activer les macros; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | Définit l'onglet de feuille de calcul visible en premier. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Définit les paramètres de mondialisation. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indique si ce classeur est masqué. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Définit si la liste des champs du tableau croisé dynamique doit être masquée. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Définit la langue de l’interface utilisateur de la version du Workbook basée sur CountryCode qui a enregistré le fichier. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Définit la langue utilisée par ce classeur. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Définit le numéro maximal de ligne de la formule partagée. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Définit la limitation d'éléments uniques par champ |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Définit les options d'utilisation de la mémoire. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Représente si la feuille de calcul générée sera ouverte minimisée. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Définit le caractère qui sépare les groupes de chiffres à gauche du séparateur décimal dans les valeurs numériques. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Définit le type d'orientation d'impression pour l'ensemble du classeur. |
| [setPaperSize(int value)](#setPaperSize-int-) | Définit la taille de papier d'impression par défaut. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Représente le mot de passe de chiffrement du fichier Workbook. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Indique si les propriétés des points de données et les étiquettes de données dans tous les graphiques de ce Workbook suivent leur référence. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Indique si la définition de la propriété [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) lors de la saisie de la valeur chaîne (qui commence par une apostrophe) dans la cellule |
| [setRegion(int value)](#setRegion-int-) | Définit les paramètres régionaux du classeur. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | Vrai si les informations personnelles peuvent être supprimées du Workbook spécifié. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Indique si l'application a ouvert le Workbook en dernier en mode sécurisé ou de réparation. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Définit le fournisseur de flux pour les ressources externes, comme le chargement de données d'image pour une image de type \"LinkToFile\". |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | Définit comment l'application affiche les formes dans ce classeur |
| [setShared(boolean value)](#setShared-boolean-) | Définit une valeur indiquant si le classeur est partagé. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Largeur de la barre d'onglets de la feuille de calcul (en 1/1000 de la largeur de la fenêtre). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Définit une valeur indiquant si les onglets du classeur sont affichés. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Définit le nombre de chiffres significatifs. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Définit le type de chiffres significatifs pour la sortie des valeurs numériques dans ce classeur. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Définit le fournisseur de flux pour les ressources externes. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Indique si la bordure des cellules adjacentes est mise à jour. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Définit comment les liens externes sont mis à jour lorsque le classeur est ouvert. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | La hauteur de la fenêtre, en points. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | La hauteur de la fenêtre, en centimètres. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | La hauteur de la fenêtre, en unité de pouce. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre, en unité de point. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. |
| [setWindowTop(double value)](#setWindowTop-double-) | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de point. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de centimètre. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de pouce. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | La largeur de la fenêtre, en unité de point. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | La largeur de la fenêtre, en unité de centimètre. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | La largeur de la fenêtre, en unité de pouce. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Indique si la compatibilité avec WPS doit être activée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Libère les ressources.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Obtient l'auteur du fichier.

**Remarks**

Ce n'est pas défini, vérifiez d'abord [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\\#getAuthor--) puis vérifiez l'utilisateur de Environment.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Indique si le fichier est marqué pour la récupération automatique.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Spécifie la version publique incrémentale de l'application.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Indique s'il faut vérifier la compatibilité avec les versions antérieures lors de l'enregistrement du classeur.

**Remarks**

La valeur par défaut est true. Seulement pour les fichiers Excel97-2003 xls ou xlt.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Indique s'il faut vérifier le format numérique personnalisé lors du réglage de Style.Custom.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Spécifie la version OOXML pour le document de sortie. La valeur par défaut est Ecma376\\_2006.

Voir [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Uniquement pour les fichiers .xlsx.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


indique si l'application a enregistré le fichier du classeur après un plantage.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


indique si l'application a ouvert le classeur pour la récupération des données.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Obtient une valeur qui représente si le classeur utilise le système de dates 1904.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Obtient la résolution par défaut de l'image.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Obtient les paramètres des valeurs par défaut des propriétés liées au style pour ce classeur.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Indique s'il faut abandonner les données d'image en cours d'édition.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Indique si et comment afficher les objets dans le classeur.

Voir [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Activer les macros;

**Remarks**

Cela ne fonctionne maintenant que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


Obtient le premier onglet de feuille de calcul visible.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Obtient les paramètres des fonctionnalités liées aux formules.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Obtient les paramètres de mondialisation.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


Obtient si la liste des champs du tableau croisé dynamique est masquée.

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
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Obtient la locale utilisée par ce classeur.

**Remarks**

Renvoie null si ni Locale ni [getRegion()](../../com.aspose.cells/workbooksettings\\#getRegion--) n'est défini.

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Obtient l'index maximal de colonne, basé sur zéro.

**Remarks**

Renvoie 255 si le format de fichier est Excel97-2003 ;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Obtient l'index maximal de ligne, basé sur zéro.

**Remarks**

Renvoie 65535 si le format de fichier est Excel97-2003 ;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Obtient le numéro maximal de ligne de la formule partagée.

**Remarks**

Si le nombre est trop grand, l’autofilter fonctionne très lentement dans MS Excel 2013.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Obtient la limitation des éléments uniques par champ

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Obtient les options d’utilisation de la mémoire. La nouvelle option sera prise comme option par défaut pour les feuilles de calcul nouvellement créées mais ne prendra pas effet pour les feuilles de calcul existantes.

Voir [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Pour plus de détails sur le mode mémoire, veuillez consulter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Obtient le séparateur décimal pour le formatage/l’analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Obtient le caractère qui sépare les groupes de chiffres à gauche du séparateur décimal dans les valeurs numériques. La valeur par défaut est le séparateur de groupe de la région actuelle.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Obtient la taille de papier d'impression par défaut.

Voir [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

S'il n'existe aucun paramètre concernant la taille du papier, MS Excel utilisera le paramètre d'imprimante par défaut.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Représente le mot de passe de chiffrement du fichier Workbook.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Indique si les propriétés des points de données et les étiquettes de données dans tous les graphiques de ce Workbook suivent leur référence.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Obtient le type de protection du Workbook.

Voir [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Indique si la définition de la propriété [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) lors de la saisie de la valeur chaîne (qui commence par une apostrophe) dans la cellule

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Obtient les paramètres régionaux du Workbook.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Paramètres régionaux utilisés par le composant Aspose.Cells pour un classeur chargé à partir d’un fichier modèle : i). Pour un fichier XLS, des champs sont définis pour les paramètres régionaux et MS Excel enregistre les données de paramètres régionaux dans le fichier lors de l’enregistrement du fichier XLS. Ainsi, nous utilisons la région enregistrée dans le fichier modèle pour le classeur. Si vous ne souhaitez pas utiliser la région enregistrée dans le fichier XLS, veuillez la réinitialiser à la valeur attendue (par exemple, CountryCode.Default) après le chargement du fichier modèle. De plus, nous enregistrons également la valeur spécifiée par l’utilisateur (via cette méthode) dans le fichier lors de l’enregistrement d’un fichier XLS. ii). Pour les autres formats de fichier, tels que XLSX, XLSB… etc., aucun champ n’est défini pour les paramètres régionaux dans la spécification du format de fichier. Ainsi, nous utilisons les paramètres régionaux de l’environnement de l’application pour le classeur. Et la valeur spécifiée par l’utilisateur (via cette méthode) ne peut pas être conservée pour les fichiers générés avec ces formats de fichier. 2. Pour l’effet d’affichage dans MS Excel : les paramètres régionaux appliqués ici ne peuvent prendre effet qu’à l’exécution avec le composant Aspose.Cells et non lors de la visualisation du fichier généré avec MS Excel. Même pour le fichier XLS généré dans lequel les données de paramètres régionaux spécifiées ont été enregistrées, lors de la visualisation/modification avec MS Excel, la région utilisée par MS Excel pour le formatage est toujours les paramètres régionaux par défaut de l’environnement où MS Excel s’exécute, et non celle enregistrée dans le fichier. C’est le comportement de MS Excel et il ne peut pas être modifié par le code.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


Vrai si les informations personnelles peuvent être supprimées du Workbook spécifié.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Indique si l'application a ouvert le Workbook en dernier en mode sécurisé ou de réparation.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Obtient le fournisseur de flux pour la ressource externe, comme le chargement des données d'image pour une image de type "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


Obtient la façon dont l'application affiche les formes dans ce Workbook

Voir [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


Obtient une valeur indiquant si le Workbook est partagé.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Largeur de la barre d'onglets de la feuille de calcul (en 1/1000 de la largeur de la fenêtre).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Obtient une valeur indiquant si les onglets du Workbook sont affichés.

**Remarks**

La valeur par défaut est true.

**Example**

Le code suivant masque les onglets de feuille et les boutons de défilement d’onglet pour la feuille de calcul.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Obtient le nombre de chiffres significatifs. La valeur par défaut est [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Peut uniquement être 15 ou 17 actuellement. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Cette propriété sera supprimée 12 mois plus tard à compter de juin 2025. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Obtient le type de chiffres significatifs pour la sortie des valeurs numériques dans ce classeur. La valeur par défaut est [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Voir [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Obtient les options de la balise intelligente.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Obtient le fournisseur de flux pour la ressource externe.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ResourceProvider. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2022. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Obtient le nom de police du thème par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). Le type de schéma de la police. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Indique si la bordure des cellules adjacentes est mise à jour.

**Remarks**

La valeur par défaut est false. Par exemple : la bordure inférieure de la cellule A1 est mise à jour, la bordure supérieure de la cellule A2 doit également être modifiée.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Obtient la façon dont les liens externes sont mis à jour lorsque le Workbook est ouvert.

Voir [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtient le rappel d'avertissement.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


La hauteur de la fenêtre, en points.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


La hauteur de la fenêtre, en centimètres.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


La hauteur de la fenêtre, en unité de pouce.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre, en unité de point.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En centimètres.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En pouces.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de point.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de centimètre.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de pouce.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


La largeur de la fenêtre, en unité de point.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


La largeur de la fenêtre, en unité de centimètre.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


La largeur de la fenêtre, en unité de pouce.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Indique si la compatibilité avec WPS doit être activée.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Fournit l'accès aux options de protection en écriture du classeur.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Indique si le classeur doit être chiffré avec le mot de passe par défaut lorsque la structure et les fenêtres du classeur sont verrouillés.

**Remarks**

La valeur par défaut est false maintenant. C’est identique à MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Obtient une valeur qui indique si un mot de passe est requis pour ouvrir ce classeur.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Obtient une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale.

**Remarks**

La valeur par défaut est true.

**Example**

Le code suivant rend la barre de défilement horizontale invisible pour la feuille de calcul.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indique si ce classeur est masqué.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Représente si la feuille de calcul générée sera ouverte minimisée.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Obtient une valeur qui indique si la structure ou la fenêtre du classeur est protégée.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Obtient une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale.

**Remarks**

La valeur par défaut est true.

**Example**

Le code suivant rend la barre de défilement verticale invisible pour la feuille de calcul.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Définit l'auteur du fichier.

**Remarks**

Ce n'est pas défini, vérifiez d'abord [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\\#getAuthor--) puis vérifiez l'utilisateur de Environment.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Indique si le fichier est marqué pour la récupération automatique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Spécifie la version publique incrémentale de l'application.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Indique s'il faut vérifier la compatibilité avec les versions antérieures lors de l'enregistrement du classeur.

**Remarks**

La valeur par défaut est true. Seulement pour les fichiers Excel97-2003 xls ou xlt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Indique s'il faut vérifier le format numérique personnalisé lors du réglage de Style.Custom.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Spécifie la version OOXML pour le document de sortie. La valeur par défaut est Ecma376\\_2006.

Voir [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Uniquement pour les fichiers .xlsx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


indique si l'application a enregistré le fichier du classeur après un plantage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


indique si l'application a ouvert le classeur pour la récupération des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Définit une valeur qui représente si le classeur utilise le système de date 1904.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Indique si le classeur doit être chiffré avec le mot de passe par défaut lorsque la structure et les fenêtres du classeur sont verrouillés.

**Remarks**

La valeur par défaut est false maintenant. C’est identique à MS Excel 2013.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Définit la résolution par défaut de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Indique s'il faut abandonner les données d'image en cours d'édition.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Indique si et comment afficher les objets dans le classeur.

Voir [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Activer les macros;

**Remarks**

Cela ne fonctionne maintenant que lors de la copie d'une feuille de calcul vers une autre feuille dans un classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


Définit l'onglet de feuille de calcul visible en premier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Définit les paramètres de mondialisation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale.

**Remarks**

La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indique si ce classeur est masqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Définit si la liste des champs du tableau croisé dynamique doit être masquée.

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

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Définit la langue utilisée par ce classeur.

**Remarks**

Renvoie null si ni Locale ni [getRegion()](../../com.aspose.cells/workbooksettings\\#getRegion--) n'est défini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Définit le numéro maximal de ligne de la formule partagée.

**Remarks**

Si le nombre est trop grand, l’autofilter fonctionne très lentement dans MS Excel 2013.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Définit la limitation d'éléments uniques par champ

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Définit les options d'utilisation de la mémoire. La nouvelle option sera prise comme option par défaut pour les feuilles de calcul nouvellement créées mais ne prend pas effet pour les feuilles de calcul existantes.

Voir [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

Pour plus de détails sur le mode mémoire, veuillez consulter [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Représente si la feuille de calcul générée sera ouverte minimisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Définit le caractère qui sépare les groupes de chiffres à gauche du séparateur décimal dans les valeurs numériques. La valeur par défaut est le séparateur de groupe de la région actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Définit le type d'orientation d'impression pour l'ensemble du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). Le type d'orientation de page |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Définit la taille de papier d'impression par défaut.

Voir [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

S'il n'existe aucun paramètre concernant la taille du papier, MS Excel utilisera le paramètre d'imprimante par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Représente le mot de passe de chiffrement du fichier Workbook.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Indique si les propriétés des points de données et les étiquettes de données dans tous les graphiques de ce Workbook suivent leur référence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Indique si la définition de la propriété [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) lors de la saisie de la valeur chaîne (qui commence par une apostrophe) dans la cellule

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Définit les paramètres régionaux du classeur.

Voir [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Paramètres régionaux utilisés par le composant Aspose.Cells pour un classeur chargé à partir d’un fichier modèle : i). Pour un fichier XLS, des champs sont définis pour les paramètres régionaux et MS Excel enregistre les données de paramètres régionaux dans le fichier lors de l’enregistrement du fichier XLS. Ainsi, nous utilisons la région enregistrée dans le fichier modèle pour le classeur. Si vous ne souhaitez pas utiliser la région enregistrée dans le fichier XLS, veuillez la réinitialiser à la valeur attendue (par exemple, CountryCode.Default) après le chargement du fichier modèle. De plus, nous enregistrons également la valeur spécifiée par l’utilisateur (via cette méthode) dans le fichier lors de l’enregistrement d’un fichier XLS. ii). Pour les autres formats de fichier, tels que XLSX, XLSB… etc., aucun champ n’est défini pour les paramètres régionaux dans la spécification du format de fichier. Ainsi, nous utilisons les paramètres régionaux de l’environnement de l’application pour le classeur. Et la valeur spécifiée par l’utilisateur (via cette méthode) ne peut pas être conservée pour les fichiers générés avec ces formats de fichier. 2. Pour l’effet d’affichage dans MS Excel : les paramètres régionaux appliqués ici ne peuvent prendre effet qu’à l’exécution avec le composant Aspose.Cells et non lors de la visualisation du fichier généré avec MS Excel. Même pour le fichier XLS généré dans lequel les données de paramètres régionaux spécifiées ont été enregistrées, lors de la visualisation/modification avec MS Excel, la région utilisée par MS Excel pour le formatage est toujours les paramètres régionaux par défaut de l’environnement où MS Excel s’exécute, et non celle enregistrée dans le fichier. C’est le comportement de MS Excel et il ne peut pas être modifié par le code.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


Vrai si les informations personnelles peuvent être supprimées du Workbook spécifié.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Indique si l'application a ouvert le Workbook en dernier en mode sécurisé ou de réparation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Définit le fournisseur de flux pour les ressources externes, comme le chargement de données d'image pour une image de type \"LinkToFile\".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


Définit comment l'application affiche les formes dans ce classeur

Voir [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Définit une valeur indiquant si le classeur est partagé.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Largeur de la barre d'onglets de la feuille de calcul (en 1/1000 de la largeur de la fenêtre).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Définit une valeur indiquant si les onglets du classeur sont affichés.

**Remarks**

La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Définit le nombre de chiffres significatifs. La valeur par défaut est [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Peut uniquement être 15 ou 17 actuellement. NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Cette propriété sera supprimée 12 mois plus tard à compter de juin 2025. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Définit le type de chiffres significatifs pour la sortie des valeurs numériques dans ce classeur. La valeur par défaut est [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Voir [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Définit le fournisseur de flux pour les ressources externes.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ResourceProvider. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2022. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Indique si la bordure des cellules adjacentes est mise à jour.

**Remarks**

La valeur par défaut est false. Par exemple : la bordure inférieure de la cellule A1 est mise à jour, la bordure supérieure de la cellule A2 doit également être modifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Définit comment les liens externes sont mis à jour lorsque le classeur est ouvert.

Voir [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale.

**Remarks**

La valeur par défaut est true.

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


La hauteur de la fenêtre, en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


La hauteur de la fenêtre, en centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


La hauteur de la fenêtre, en unité de pouce.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre, en unité de point.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En centimètres.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En pouces.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de point.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de centimètre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de pouce.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


La largeur de la fenêtre, en unité de point.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


La largeur de la fenêtre, en unité de centimètre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


La largeur de la fenêtre, en unité de pouce.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Indique si la compatibilité avec WPS doit être activée.

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

