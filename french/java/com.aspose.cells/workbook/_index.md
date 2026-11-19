---
title: "Workbook"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un objet racine pour créer une feuille de calcul Excel."
type: docs
url: /fr/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Représente un objet racine pour créer une feuille de calcul Excel.

**Remarks**

La classe Workbook désigne une feuille de calcul Excel. Chaque feuille de calcul peut contenir plusieurs feuilles de calcul. La fonctionnalité de base de la classe est d'ouvrir et d'enregistrer des fichiers Excel natifs. La classe possède des fonctionnalités avancées telles que la copie de données à partir d'autres Workbooks, la combinaison de deux Workbooks, la conversion d'Excel en PDF, le rendu d'Excel en image et la protection de la feuille de calcul Excel.

**Example**

L'exemple suivant charge un Workbook à partir d'un fichier Excel nommé designer.xls et rend les barres de défilement horizontales et verticales invisibles. Il remplace ensuite deux valeurs de chaîne par une valeur entière et une valeur de chaîne respectivement dans la feuille de calcul, puis enregistre finalement le classeur au format Excel xlsx.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Workbook()](#Workbook--) | Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(int fileFormatType)](#Workbook-int-) | Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | Initialise une nouvelle instance vide de la classe [Workbook](../../com.aspose.cells/workbook) avec des options |
| [Workbook(String file)](#Workbook-java.lang.String-) | Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre un fichier. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre un flux. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre un fichier. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre le flux. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Accepte toutes les modifications suivies dans le classeur. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Ajoute une signature numérique à un fichier de feuille de calcul OOXML (Excel2007 et versions ultérieures). |
| [calculateFormula()](#calculateFormula--) | Calcule le résultat des formules. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Calcule le résultat des formules. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Calcul des formules dans ce classeur. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Modifie la palette de la feuille de calcul à l'index spécifié. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Ferme la session qui utilise des caches pour accéder aux données. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Combine un autre objet Workbook. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Copie les données d'un objet Workbook source. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Copie un autre objet Workbook. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Copie le thème d'un autre classeur. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Crée un style intégré selon le type donné. |
| [createCellsColor()](#createCellsColor--) | Crée un objet [CellsColor](../../com.aspose.cells/cellscolor). |
| [createStyle()](#createStyle--) | Crée un nouveau style. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | Crée un nouveau style. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Personnalise le thème. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Exporte les données XML liées par la carte XML spécifiée. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Exporte les données XML liées par la carte XML spécifiée. |
| [getAbsolutePath()](#getAbsolutePath--) | Obtient le chemin absolu du fichier. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document intégrées de la feuille de calcul. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Obtient la fabrique pour créer ICellsDataTable à partir d'objets personnalisés |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Renvoie les couleurs de la palette pour la feuille de calcul. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Obtient la liste des objets [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) dans le classeur. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Obtient le nombre de styles dans le pool de styles. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document personnalisées de la feuille de calcul. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Représente un Custom XML Data Storage Part (custom XML data within a package). |
| [getDataConnections()](#getDataConnections--) | Obtient la collection [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getDataMashup()](#getDataMashup--) | Obtient les données mashup. |
| [getDataModel()](#getDataModel--) | Obtient le modèle de données dans le classeur. |
| [getDataSorter()](#getDataSorter--) | Obtient un objet DataSorter pour trier les données. |
| [getDefaultStyle()](#getDefaultStyle--) | Obtient l'objet [Style](../../com.aspose.cells/style) par défaut du classeur. |
| [getDigitalSignature()](#getDigitalSignature--) | Obtient la signature numérique du fichier. |
| [getFileFormat()](#getFileFormat--) | Obtient le format du fichier. |
| [getFileName()](#getFileName--) | Obtient le nom de fichier actuel. |
| [getFonts()](#getFonts--) | Obtient toutes les polices dans le pool de styles. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Obtient le moniteur d'interruption. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Trouve la couleur la plus proche dans la palette actuelle. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Obtient le style nommé dans le pool de styles. |
| [getRibbonXml()](#getRibbonXml--) | Obtient le fichier XML qui définit l'interface du Ruban. |
| [getSettings()](#getSettings--) | Représente les paramètres du classeur. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Obtient le style dans le pool de styles. |
| [getTheme()](#getTheme--) | Obtient le nom du thème. |
| [getThemeColor(int type)](#getThemeColor-int-) | Obtient la couleur du thème. |
| [getVbaProject()](#getVbaProject--) | Obtient le [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) dans une feuille de calcul. |
| [getWorksheets()](#getWorksheets--) | Obtient la collection [WorksheetCollection](../../com.aspose.cells/worksheetcollection) dans la feuille de calcul. |
| [hasCustomFunction()](#hasCustomFunction--) | Détecte s'il y a une fonction personnalisée utilisée dans ce classeur, comme dans la formule d'une cellule, dans les noms définis... |
| [hasExernalLinks()](#hasExernalLinks--) | Indique si ce classeur contient des liens externes vers d'autres sources de données. |
| [hasMacro()](#hasMacro--) | Indique si cette feuille de calcul contient des macros/VBA. |
| [hasRevisions()](#hasRevisions--) | Obtient si le classeur possède des modifications suivies |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Vérifie si une couleur est dans la palette de la feuille de calcul. |
| [isDigitallySigned()](#isDigitallySigned--) | Indique si cette feuille de calcul est signée numériquement. |
| [isLicensed()](#isLicensed--) | Indique si la licence est définie. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Indique si la structure ou la fenêtre est protégée par mot de passe. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | Fusionne les styles nommés du autre fichier Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées depuis le fichier modèle ou affectées à une cellule. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Protège un classeur. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Protège un classeur partagé. |
| [refreshAll()](#refreshAll--) | Actualiser les formes liées, tous les tableaux croisés dynamiques et les graphiques avec la source du tableau croisé dynamique. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines selon les données actuelles). Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules de tableau dynamique. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines selon les données actuelles). |
| [removeDigitalSignature()](#removeDigitalSignature--) | Supprime la signature numérique de cette feuille de calcul. |
| [removeExternalLinks()](#removeExternalLinks--) | Supprime tous les liens externes du classeur. |
| [removeMacro()](#removeMacro--) | Supprime le VBA/macro de cette feuille de calcul. |
| [removePersonalInformation()](#removePersonalInformation--) | Supprime les informations personnelles. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Supprime tous les styles inutilisés. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Remplace les valeurs des cellules par de nouvelles données. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Remplace les valeurs des cellules par de nouvelles données. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Remplace la valeur d'une cellule par un nouveau double. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Remplace les valeurs des cellules par un tableau de doubles. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Remplace la valeur d'une cellule par un nouvel entier. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Remplace les valeurs des cellules par un tableau d'entiers. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Remplace la valeur d'une cellule par un nouveau tableau de chaînes. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Enregistre le classeur dans le flux. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Enregistre le classeur dans le flux. |
| [save(String fileName)](#save-java.lang.String-) | Enregistre le classeur sur le disque. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Enregistre le classeur sur le disque. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Enregistre le classeur sur le disque. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | Définit le chemin absolu du fichier. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | Définit l'objet [Style](../../com.aspose.cells/style) par défaut du classeur. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Définit la signature numérique d'un fichier de feuille de calcul (Excel2007 et versions ultérieures). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Définir les options de chiffrement. |
| [setFileFormat(int value)](#setFileFormat-int-) | Définit le format du fichier. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Définit le nom du fichier actuel. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Définit le moniteur d’interruption. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | Définit le fichier XML qui définit l'interface du ruban. |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Définit la couleur du thème |
| [startAccessCache(int opts)](#startAccessCache-int-) | Démarre la session qui utilise des caches pour accéder aux données. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Supprime la protection d’un classeur. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Supprime la protection d’un classeur partagé. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Met à jour la définition des fonctions personnalisées. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | Si ce classeur contient des liens externes vers d’autres sources de données, Aspose.Cells tentera de récupérer les dernières données à partir des sources fournies. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Le type de format de fichier par défaut est Xlsx. Si vous souhaitez créer d’autres types de fichiers, veuillez utiliser Workbook(FileFormatType).

**Example**

Le code suivant montre comment utiliser le constructeur Workbook pour créer et initialiser une nouvelle instance de la classe.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Le type de format de fichier par défaut est Excel97To2003.

**Example**

Le code suivant montre comment utiliser le constructeur Workbook pour créer et initialiser une nouvelle instance de la classe avec différents types de format de fichier.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). Le nouveau format de fichier. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


Initialise une nouvelle instance vide de la classe [Workbook](../../com.aspose.cells/workbook) avec des options

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Les options. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fichier | java.lang.String | Le nom du fichier. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre un fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fichier | java.lang.String | Le nom du fichier. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Les options de chargement |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [Workbook](../../com.aspose.cells/workbook) et ouvre le flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Les options de chargement |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Accepte toutes les modifications suivies dans le classeur.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Ajoute une signature numérique à un fichier de feuille de calcul OOXML (Excel2007 et versions ultérieures).

**Remarks**

Prend en charge uniquement l’ajout de la signature numérique Xmldsig à un fichier de feuille de calcul OOXML

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcule le résultat des formules.

**Remarks**

Pour toutes les formules prises en charge, veuillez consulter la liste à https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Calcule le résultat des formules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Indique s’il faut masquer l’erreur lors du calcul des formules. L’erreur peut être due à une fonction non prise en charge, des liens externes, etc. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Calcul des formules dans ce classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options de calcul |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Modifie la palette de la feuille de calcul à l'index spécifié.

**Remarks**

La palette comporte 56 entrées, chacune représentée par une valeur RVB.

Si vous définissez une couleur qui n’est pas dans la palette, elle ne prendra pas effet.

Donc, si vous souhaitez définir une couleur personnalisée, veuillez d’abord modifier la palette.

Ce qui suit est la palette de couleurs standard.

| Couleur | Rouge | Vert | Bleu |
| ------- | --- | ----- | ---- |
| Noir | 0 | 0 | 0 |
| Blanc | 255 | 255 | 255 |
| Rouge | 255 | 0 | 0 |
| Citron vert | 0 | 255 | 0 |
| Bleu | 0 | 0 | 255 |
| Jaune | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Cyan | 0 | 255 | 255 |
| Marron | 128 | 0 | 0 |
| Vert | 0 | 128 | 0 |
| Marine | 0 | 0 | 128 |
| Olive | 128 | 128 | 0 |
| Violet | 128 | 0 | 128 |
| Sarcelle | 0 | 128 | 128 |
| Argent | 192 | 192 | 192 |
| Gris | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Couleur22 | 255 | 128 | 128 |
| Couleur23 | 0 | 102 | 204 |
| Couleur24 | 204 | 204 | 255 |
| Couleur25 | 0 | 0 | 128 |
| Couleur26 | 255 | 0 | 255 |
| Couleur27 | 255 | 255 | 0 |
| Couleur28 | 0 | 255 | 255 |
| Couleur29 | 128 | 0 | 128 |
| Couleur30 | 128 | 0 | 0 |
| Couleur31 | 0 | 128 | 128 |
| Couleur32 | 0 | 0 | 255 |
| Couleur33 | 0 | 204 | 255 |
| Couleur34 | 204 | 255 | 255 |
| Couleur35 | 204 | 255 | 204 |
| Couleur36 | 255 | 255 | 153 |
| Couleur37 | 153 | 204 | 255 |
| Couleur38 | 255 | 153 | 204 |
| Couleur39 | 204 | 153 | 255 |
| Couleur40 | 255 | 204 | 153 |
| Couleur41 | 51 | 102 | 255 |
| Couleur42 | 51 | 204 | 204 |
| Couleur43 | 153 | 204 | 0 |
| Couleur44 | 255 | 204 | 0 |
| Couleur45 | 255 | 153 | 0 |
| Couleur46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Structure de couleur. |
| index | int | Index de palette, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Ferme la session qui utilise des caches pour accéder aux données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). options d'accès aux données |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Combine un autre objet Workbook.

**Remarks**

Fusionner Excel, ODS, CSV et d'autres fichiers en un seul fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | Un autre objet Workbook. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Copie les données d'un objet Workbook source.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Objet Workbook source. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Copie un autre objet Workbook.

**Remarks**

Il est très simple de cloner un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Objet Workbook source. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Les options de copie d'un autre classeur. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Copie le thème d'un autre classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Classeur source. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Crée un style intégré selon le type donné.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). Le style intégré. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Crée un objet [CellsColor](../../com.aspose.cells/cellscolor).

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Crée un nouveau style.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


Crée un nouveau style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cloneDefaultStyle | boolean | Indique si le style par défaut est cloné |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Personnalise le thème.

**Remarks**

La longueur des couleurs doit être de 12.

| Indice de tableau | Type de thème |
| ----------- | ------------------ |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Lien hypertexte |
| 11 | Lien hypertexte visité |

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| themeName | java.lang.String | Le nom du thème |
| colors | [Color\[\]](../../com.aspose.cells/color) | Les couleurs du thème |

### dispose() {#dispose--}
```
public void dispose()
```


Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées.

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Exporte les données XML liées par la carte XML spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| mapName | java.lang.String | nom de la carte XML qui doit être exportée |
| stream | java.io.OutputStream | le flux d'exportation |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Exporte les données XML liées par la carte XML spécifiée.

**Example**

Le code suivant a exporté les données liées par le premier XmlMap.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| mapName | java.lang.String | nom de la carte XML qui doit être exportée |
| chemin | java.lang.String | le chemin d'exportation |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


Obtient le chemin absolu du fichier.

**Remarks**

Utilisé uniquement pour les liens externes.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document intégrées de la feuille de calcul.

**Remarks**

Une nouvelle propriété ne peut pas être ajoutée à la liste des propriétés de document intégrées. Vous ne pouvez que récupérer une propriété intégrée et modifier sa valeur. La liste suivante présente les noms des propriétés intégrées :

Title

Sujet

Auteur

Mots-clés

Commentaires

Modèle

Dernier auteur

Numéro de révision

Nom de l'application

Date de la dernière impression

Date de création

Heure du dernier enregistrement

Temps total d'édition

Nombre de pages

Nombre de mots

Nombre de caractères

Sécurité

Catégorie

Format

Gestionnaire

Entreprise

Nombre d'octets

Nombre de lignes

Nombre de paragraphes

Nombre de diapositives

Nombre de notes

Nombre de diapositives masquées

Nombre de clips multimédias

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Obtient la fabrique pour créer ICellsDataTable à partir d'objets personnalisés

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Renvoie les couleurs de la palette pour la feuille de calcul.

**Remarks**

La palette comporte 56 entrées, chacune représentée par une valeur RVB.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Obtient la liste des objets [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) dans le classeur.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Obtient le nombre de styles dans le pool de styles.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Renvoie une collection de [DocumentProperty](../../com.aspose.cells/documentproperty) qui représente toutes les propriétés de document personnalisées de la feuille de calcul.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Représente un Custom XML Data Storage Part (custom XML data within a package).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


Obtient la collection [ExternalConnection](../../com.aspose.cells/externalconnection).

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Obtient les données mashup.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


Obtient le modèle de données dans le classeur.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Obtient un objet DataSorter pour trier les données.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


Obtient l'objet [Style](../../com.aspose.cells/style) par défaut du classeur.

**Remarks**

La propriété DefaultStyle est utile pour implémenter un Style pour l'ensemble du Workbook.

**Example**

Le code suivant crée et instancie un nouveau Workbook et définit un [Style](../../com.aspose.cells/style) par défaut.

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Obtient la signature numérique du fichier.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Obtient le format du fichier.

Voir [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


Obtient le nom de fichier actuel.

**Remarks**

Si le fichier est ouvert par flux et qu'il existe des références de formules externes, veuillez définir le nom du fichier.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Obtient toutes les polices dans le pool de styles.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Obtient le moniteur d'interruption.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Trouve la couleur la plus proche dans la palette actuelle.

**Remarks**

Il n'y a que 56 couleurs dans la palette de couleurs d'Excel 97-2003. Si la couleur n'est pas dans la palette, une couleur similaire sera définie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Couleur brute. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Obtient le style nommé dans le pool de styles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | nom du style |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


Obtient le fichier XML qui définit l'interface du Ruban.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Représente les paramètres du classeur.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Obtient le style dans le pool de styles. Tous les styles du classeur seront rassemblés dans un pool. Il n'y a qu'un simple index de référence dans les cellules.

**Remarks**

Si le style retourné est modifié, le style de toutes les cellules (qui font référence à ce style) sera modifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Obtient le nom du thème.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Obtient la couleur du thème.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Le type de couleur du thème. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Obtient le [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) dans une feuille de calcul.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Obtient la collection [WorksheetCollection](../../com.aspose.cells/worksheetcollection) dans la feuille de calcul.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Détecte s'il y a une fonction personnalisée utilisée dans ce classeur, comme dans la formule d'une cellule, dans les noms définis...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Indique si ce classeur contient des liens externes vers d'autres sources de données.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser ExternalLinkCollection.Count pour vérifier s'il y a des liens externes dans ce classeur. Cette méthode sera supprimée 12 mois plus tard à compter de décembre 2021. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
booléen - Indique si ce classeur contient des liens externes vers d'autres sources de données.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Indique si cette feuille de calcul contient des macros/VBA.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Obtient si le classeur possède des modifications suivies

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Importe/Met à jour un fichier de données XML dans le classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | le flux du fichier xml. |
| sheetName | java.lang.String | le nom de la feuille de destination. |
| ligne | int | la ligne de destination. |
| col | int | la colonne de destination. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Importe/Met à jour un fichier de données XML dans le classeur.

**Example**

Le code suivant importe des données XML dans la feuille de calcul 'Sheet 1' à la cellule A1.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| url | java.lang.String | l'URL/chemin du fichier XML. |
| sheetName | java.lang.String | le nom de la feuille de destination. |
| ligne | int | la ligne de destination |
| col | int | la colonne de destination |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Vérifie si une couleur est dans la palette de la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Structure de couleur. |

**Returns:**
booléen - Retourne vrai si cette couleur est dans la palette. Sinon, retourne faux
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Indique si cette feuille de calcul est signée numériquement.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Indique si la licence est définie.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Indique si la structure ou la fenêtre est protégée par mot de passe.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


Fusionne les styles nommés du autre fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | L'autre fichier |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées depuis le fichier modèle ou affectées à une cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Indique s'il faut ignorer les erreurs pour une formule invalide. Pour une formule invalide, si l'erreur est ignorée, alors cette formule sera ignorée et le processus continuera à analyser les autres formules, sinon une exception sera levée. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Protège un classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Type de protection. |
| password | java.lang.String | Mot de passe pour protéger le classeur. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Protège un classeur partagé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Mot de passe pour protéger le classeur. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Actualiser les formes liées, tous les tableaux croisés dynamiques et les graphiques avec la source du tableau croisé dynamique.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines selon les données actuelles). Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules de tableau dynamique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| calculer | boolean | Indique s'il faut calculer et mettre à jour les valeurs des cellules pour ces formules de tableau dynamique |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines selon les données actuelles).

**Remarks**

Pour des raisons de performance, nous ne rafraîchissons pas automatiquement toutes les formules de tableau dynamique lorsque la formule elle-même ou les données auxquelles elle fait référence sont modifiées. L'utilisateur doit donc appeler cette méthode manuellement après les opérations susceptibles d'influencer les formules de tableau dynamique, telles que l'importation/la définition de valeurs de cellules, l'insertion/la suppression de lignes/colonnes/plages, etc.

Pour la plupart des formules contenant des fonctions, le calcul de la zone de débordement nécessite également le calcul de la formule, ainsi, en général, la valeur true du drapeau "calculate" est préférée. Si la formule est simple, comme une référence de plage ou un tableau (par exemple "=C1:E5", "=\\{1,2;3,4\\}", ...), une fonction simple sur une plage ou un tableau (par exemple "=ABS(C1:E5)", "=1+\\{1,2;3,4\\}", ...), et que toutes les formules seront calculées ultérieurement (par exemple via [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\\#calculateFormula-CalculationOptions-)), alors utiliser la valeur false pour le drapeau "calculate" peut éviter le calcul dupliqué au profit des performances.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| calculer | boolean | Indique s'il faut calculer et mettre à jour les valeurs des cellules pour ces formules de tableau dynamique |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Les options de calcul des formules |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Supprime la signature numérique de cette feuille de calcul.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Supprime tous les liens externes du classeur.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la méthode ExternalLinkCollection.Clear(). Cette méthode sera supprimée 12 mois après décembre 2021. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Supprime le VBA/macro de cette feuille de calcul.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Supprime les informations personnelles.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Supprime tous les styles inutilisés.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Remplace les valeurs des cellules par de nouvelles données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| boolValue | boolean | La valeur booléenne à remplacer. |
| newValue | java.lang.Object | Nouvelle valeur. Peut être une chaîne, un entier, un double ou une valeur DateTime. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Remplace les valeurs des cellules par de nouvelles données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| intValue | int | La valeur entière à remplacer. |
| newValue | java.lang.Object | Nouvelle valeur. Peut être une chaîne, un entier, un double ou une valeur DateTime. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Remplace la valeur d'une cellule par un nouveau double.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValue | double | Valeur double à remplacer |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Remplace les valeurs des cellules par un tableau de doubles.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValues | double[] | Tableau de doubles à remplacer |
| isVertical | boolean | Vrai - Vertical, Faux - Horizontal |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Remplace la valeur d'une cellule par un nouvel entier.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValue | int | Valeur entière à remplacer |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Remplace les valeurs des cellules par un tableau d'entiers.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValues | int[] | Tableau d'entiers à remplacer |
| isVertical | boolean | Vrai - Vertical, Faux - Horizontal |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Remplace la valeur d'une cellule par une nouvelle chaîne.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValue | java.lang.String | Valeur de chaîne à remplacer |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Remplace la valeur d'une cellule par une nouvelle chaîne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValue | java.lang.String | Valeur de chaîne à remplacer |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Les options de remplacement |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Remplace la valeur d'une cellule par un nouveau tableau de chaînes.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Espace réservé de cellule |
| newValues | java.lang.String[] | Tableau de chaînes à remplacer |
| isVertical | boolean | Vrai - Vertical, Faux - Horizontal |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Enregistre le classeur dans le flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de fichier. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Les options d'enregistrement. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Enregistre le classeur dans le flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de fichier. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le type de format de fichier d'enregistrement. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Enregistre le classeur sur le disque.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Enregistre le classeur sur le disque.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Les options d'enregistrement. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Enregistre le classeur sur le disque.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le type de format d'enregistrement. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


Définit le chemin absolu du fichier.

**Remarks**

Utilisé uniquement pour les liens externes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


Définit l'objet [Style](../../com.aspose.cells/style) par défaut du classeur.

**Remarks**

La propriété DefaultStyle est utile pour implémenter un Style pour l'ensemble du Workbook.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Définit la signature numérique d'un fichier de feuille de calcul (Excel2007 et versions ultérieures).

**Remarks**

Prise en charge uniquement de l'ajout de la signature numérique Xmldsig

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Définir les options de chiffrement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). Le type de chiffrement. |
| keyLength | int | La longueur de la clé. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


Définit le format du fichier.

Voir [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


Définit le nom du fichier actuel.

**Remarks**

Si le fichier est ouvert par flux et qu'il existe des références de formules externes, veuillez définir le nom du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Définit le moniteur d’interruption.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


Définit le fichier XML qui définit l'interface du ruban.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Définit la couleur du thème

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Le type de couleur du thème. |
| color | [Color](../../com.aspose.cells/color) | la couleur du thème |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Démarre la session qui utilise des caches pour accéder aux données.

**Remarks**

Si le cache d'accès aux données spécifiées nécessite que certains modèles de données dans la feuille de calcul soient en lecture seule, alors les modèles de données correspondants dans chaque feuille de calcul de ce classeur seront considérés comme en lecture seule et l'utilisateur ne doit modifier aucun d'eux.

Après avoir terminé l'accès aux données, [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) doit être invoqué avec les mêmes options pour effacer tous les caches et rétablir le mode d'accès normal.



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). options d'accès aux données |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Supprime la protection d’un classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Mot de passe pour désactiver la protection du classeur. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Supprime la protection d’un classeur partagé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Mot de passe pour désactiver la protection du classeur. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


Met à jour la définition des fonctions personnalisées.

**Remarks**

Cette méthode peut être utilisée pour certains scénarios spéciaux. Par exemple, si l'utilisateur a besoin que certains paramètres de fonctions personnalisées soient calculés en mode tableau, il peut fournir sa propre définition avec l'implémentation de [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) pour ces fonctions. Après la mise à jour des données des formules, ces paramètres spécifiés seront calculés automatiquement en mode tableau lors du calcul des fonctions personnalisées correspondantes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | Définition spéciale de fonctions personnalisées pour les exigences particulières de l'utilisateur. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


Si ce classeur contient des liens externes vers d’autres sources de données, Aspose.Cells tentera de récupérer les dernières données à partir des sources fournies.

**Remarks**

Si le lien externe correspondant ne peut pas être trouvé pour un classeur, alors ce classeur sera ignoré. Ainsi, lorsque vous définissez plus tard une formule avec un nouveau lien externe que vous souhaitez associer au classeur ignoré, le lien ne pourra pas être effectué tant que vous n'aurez pas appelé à nouveau cette méthode avec ces classeurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | Classeur(s) qui seront utilisés pour mettre à jour les données des liens externes référencés par ce classeur. L'association de ces classeurs avec les liens externes est déterminée par [getFileName()](../../com.aspose.cells/workbook\#getFileName--) et [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Veuillez donc vous assurer que [getFileName()](../../com.aspose.cells/workbook\#getFileName--) a été spécifié avec la valeur appropriée pour chaque classeur afin qu'ils puissent être liés au lien externe correspondant. |

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

