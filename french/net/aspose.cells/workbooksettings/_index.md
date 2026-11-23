---
title: "Classe WorkbookSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WorkbookSettings. Représente tous les paramètres du classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Représente tous les paramètres du classeur.

```csharp
public class WorkbookSettings : IDisposable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Obtient et définit l'auteur du fichier. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Indique si le fichier est marqué pour la récupération automatique. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Spécifie la version publique incrémentielle de l'application. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Indique si la compatibilité avec les versions antérieures est vérifiée lors de l'enregistrement du workbook. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Indique si la vérification du format numérique personnalisé est effectuée lors du paramétrage de Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Spécifie la version OOXML du document de sortie. La valeur par défaut est Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | Indique si l'application a enregistré le fichier du workbook après un plantage. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Obtient ou définit les informations de culture du système. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | Indique si l'application a ouvert le workbook pour la récupération de données. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Obtient ou définit une valeur indiquant si le workbook utilise le système de dates 1904. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Obtient et définit la résolution par défaut de l'image. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Obtient les paramètres des valeurs par défaut des propriétés liées au style pour ce workbook. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Indique si les données d'image en cours d'édition sont abandonnées. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Indique si et comment afficher les objets dans le workbook. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Activer les macros ; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | Obtient ou définit le premier onglet de feuille de calcul visible. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Obtient les paramètres des fonctionnalités liées aux formules. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Obtient et définit les paramètres de mondialisation. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | Obtient et définit si la liste des champs du PivotTable est masquée. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Indique si le workbook est chiffré avec le mot de passe par défaut lorsque la Structure et les Fenêtres du workbook sont verrouillées. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Obtient une valeur indiquant si un mot de passe est requis pour ouvrir ce workbook. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Indique si ce workbook est masqué. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Représente si la feuille de calcul générée sera ouverte minimisée. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Obtient une valeur indiquant si la structure ou la fenêtre du Workbook est protégée. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Obtient l'index maximal de colonne, basé sur zéro. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Obtient l'index maximal de ligne, basé sur zéro. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Obtient et définit le numéro maximal de ligne de la formule partagée. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Obtient et définit la limitation d'éléments uniques par champ |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Obtient ou définit les options d'utilisation de la mémoire. La nouvelle option sera prise comme option par défaut pour les feuilles de calcul nouvellement créées mais ne prendra pas effet pour les feuilles de calcul existantes. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Obtient ou définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Obtient ou définit le caractère qui sépare les groupes de chiffres à gauche du séparateur décimal dans les valeurs numériques. La valeur par défaut est le séparateur de groupe de la région actuelle. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Obtient et définit la taille de papier d'impression par défaut. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Représente le mot de passe de chiffrement du fichier du classeur. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Indique si les propriétés des points de données et les étiquettes de données dans tous les graphiques de ce classeur suivent leur référence. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Obtient le type de protection du classeur. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Indique si la définition de la propriété [`QuotePrefix`](../style/quoteprefix/) lors de la saisie de la valeur chaîne (qui commence par une apostrophe) dans la cellule. |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Obtient ou définit les paramètres régionaux du classeur. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | Vrai si les informations personnelles peuvent être supprimées du classeur spécifié. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Indique si l'application a ouvert le classeur en dernier en mode sécurisé ou de réparation. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Obtient et définit le fournisseur de flux pour les ressources externes, comme le chargement de données d'image pour une image de type "LinkToFile". |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | Obtient et définit comment l'application affiche les formes dans ce classeur. |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Obtient ou définit une valeur indiquant si le classeur est partagé. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Largeur de la barre d'onglets de la feuille de calcul (en 1/1000 de la largeur de la fenêtre). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Obtient ou définit une valeur indiquant si les onglets du classeur sont affichés. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) Obtient et définit le nombre de chiffres significatifs. La valeur par défaut est [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Obtient et définit le type de chiffres significatifs pour la sortie des valeurs numériques dans ce classeur. La valeur par défaut est [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Obtient les options de la balise intelligente. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) Obtient et définit le fournisseur de flux pour la ressource externe. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Indique si la bordure des cellules adjacentes doit être mise à jour. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Obtient et définit comment les liens externes sont mis à jour lorsque le classeur est ouvert. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | La hauteur de la fenêtre, en points. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | La hauteur de la fenêtre, en centimètres. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | La hauteur de la fenêtre, en pouces. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en points. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en centimètres. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en pouces. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en points. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en centimètres. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en pouces. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | La largeur de la fenêtre, en points. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | La largeur de la fenêtre, en centimètres. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | La largeur de la fenêtre, en pouces. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | Indique s'il faut être compatible avec WPS. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Fournit l'accès aux options de protection en écriture du classeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Libère les ressources. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Obtient le nom de police du thème par défaut. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Définit le type d'orientation d'impression pour l'ensemble du classeur. |

### Exemples

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Créer un nouveau classeur
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Ajoutez des données d'exemple
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // Accédez aux WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // Définissez divers paramètres
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Enregistrez le classeur
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


