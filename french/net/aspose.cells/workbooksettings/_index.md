---
title: WorkbookSettings
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente tous les paramètres du classeur.
type: docs
weight: 6500
url: /fr/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Représente tous les paramètres du classeur.

```csharp
public class WorkbookSettings : IDisposable
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Obtient et définit l'auteur du fichier. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Spécifie une valeur booléenne qui indique que l'application a automatiquement compressé les images dans le classeur. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Indique si le fichier est marqué pour la récupération automatique. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Spécifie la version publique incrémentielle de l'application. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Indique si vérifier la compatibilité avec les versions antérieures lors de l'enregistrement du classeur. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Indique si la vérification du format numérique personnalisé lors de la définition de Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Vérifier si la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, comme par Cell.PutValue (chaîne), si cela propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard vous puissiez sortir la valeur de chaîne complète pour d'autres formats de fichiers tels que CSV. Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement. Sinon, il peut y avoir une erreur inattendue pour le fichier Excel généré. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Spécifie la version OOXML du document de sortie. La valeur par défaut est Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | indique si l'application a enregistré le fichier de classeur pour la dernière fois après un crash. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Obtient ou définit les informations de culture système. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | indique si l'application a ouvert le classeur pour la dernière fois pour la récupération de données. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Obtient ou définit une valeur qui indique si le classeur utilise le système de date 1904. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Indique si et comment afficher les objets dans le classeur. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Activer les macros ; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | Obtient ou définit le premier onglet de feuille de calcul visible. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Obtient les paramètres des fonctionnalités liées aux formules. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Obtient et définit les paramètres de globalisation. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | Obtient et définit si masquer la liste des champs pour le tableau croisé dynamique. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Indique si le cryptage du classeur avec le mot de passe par défaut si la structure et les fenêtres du classeur sont verrouillées. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Obtient une valeur qui indique si un mot de passe est requis pour ouvrir ce classeur. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Indique si ce classeur est masqué. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Représente si la feuille de calcul générée sera ouverte réduite. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Obtient une valeur qui indique si la structure ou la fenêtre du classeur est protégée. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur en fonction du code pays qui a enregistré le fichier. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Obtient l'index de colonne maximum, basé sur zéro. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Obtient l'index de ligne maximum, basé sur zéro. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Obtient et définit le nombre maximal de lignes de la formule partagée. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Obtient ou définit les options d'utilisation de la mémoire. La nouvelle option sera considérée comme l'option par défaut pour les feuilles de calcul nouvellement créées, mais ne prend pas effet pour les feuilles de calcul existantes. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Obtient ou définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Obtient ou définit le caractère qui sépare les groupes de chiffres à gauche de la décimale dans les valeurs numériques. La valeur par défaut est le séparateur de groupe de la région actuelle. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Obtient et définit le format de papier d'impression par défaut. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Représente le mot de passe de chiffrement du fichier de classeur. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Obtient le type de protection du classeur. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Indique si le réglage[`QuotePrefix`](../style/quoteprefix) propriété lors de la saisie de la valeur de chaîne (qui commence par un guillemet simple) dans la cellule |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Obtient ou définit les paramètres régionaux du classeur. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | Vrai si les informations personnelles peuvent être supprimées du classeur spécifié. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Indique si l'application a ouvert le classeur pour la dernière fois en mode sans échec ou en mode réparation. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | Obtient et définit le fournisseur de flux pour une ressource externe, telle que le chargement de données d'image pour une image de type "LinkToFile". |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Obtient ou définit une valeur qui indique si le classeur est partagé. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Largeur de la barre d'onglets de la feuille de calcul (en 1/1000 de la largeur de la fenêtre). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Obtient ou définit une valeur indiquant si les onglets du classeur sont affichés. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Obtient et définit le nombre de chiffres significatifs. La valeur par défaut est[`SignificantDigits`](../cellshelper/significantdigits) . |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Indique si la bordure des cellules adjacentes est mise à jour. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Obtient et définit comment met à jour les liens externes lorsque le classeur est ouvert. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Obtient ou définit un rappel d'avertissement. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | La hauteur de la fenêtre, en unité de point. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | La hauteur de la fenêtre, en centimètre. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | La hauteur de la fenêtre, en unité de pouce. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre, en unité de point. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En centimètre. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | La distance entre le bord gauche de la zone client et le bord gauche de la fenêtre. En unité de pouce. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en unité de point. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en centimètre. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | La distance entre le bord supérieur de la zone client et le bord supérieur de la fenêtre, en pouces. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | La largeur de la fenêtre, en unité de point. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | La largeur de la fenêtre, en centimètre. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | La largeur de la fenêtre, en pouce. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Fournit l'accès aux options de protection en écriture du classeur. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Libère des ressources. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Obtient le nom de la police de thème par défaut. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Définir le type d'orientation d'impression pour l'ensemble du classeur. |

### Exemples

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

//faites vos affaires

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'fais ton affaire
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
