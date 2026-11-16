---
title: "Classe WorkbookSettings"
linktitle: "WorkbookSettings"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe WorkbookSettings. Encapsule l'objet qui représente les paramètres du classeur en Go."
type: docs
weight: 200
url: /fr/go-cpp/workbooksettings/
---

## WorkbookSettings class

Représente tous les paramètres du classeur.

```go

type WorkbookSettings struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [Dispose](./dispose/) | Libère les ressources. |
| [GetThemeFont](./getthemefont/) | Obtient le nom de police du thème par défaut. |
| [GetAuthor](./getauthor/) | Obtient et définit l'auteur du fichier. |
| [SetAuthor](./setauthor/) | Obtient et définit l'auteur du fichier. |
| [GetCheckCustomNumberFormat](./getcheckcustomnumberformat/) | Indique s'il faut vérifier le format numérique personnalisé lors de la définition de Style.Custom. |
| [SetCheckCustomNumberFormat](./setcheckcustomnumberformat/) | Indique s'il faut vérifier le format numérique personnalisé lors de la définition de Style.Custom. |
| [GetEnableMacros](./getenablemacros/) | Activer les macros; |
| [SetEnableMacros](./setenablemacros/) | Activer les macros; |
| [GetDate1904](./getdate1904/) | Obtient ou définit une valeur indiquant si le classeur utilise le système de dates 1904. |
| [SetDate1904](./setdate1904/) | Obtient ou définit une valeur indiquant si le classeur utilise le système de dates 1904. |
| [GetProtectionType](./getprotectiontype/) | Obtient le type de protection du classeur. |
| [GetDisplayDrawingObjects](./getdisplaydrawingobjects/) | Indique si et comment afficher les objets dans le classeur. |
| [SetDisplayDrawingObjects](./setdisplaydrawingobjects/) | Indique si et comment afficher les objets dans le classeur. |
| [GetSheetTabBarWidth](./getsheettabbarwidth/) | Largeur de la barre d'onglets de feuille de calcul (en 1/1000 de la largeur de la fenêtre). |
| [SetSheetTabBarWidth](./setsheettabbarwidth/) | Largeur de la barre d'onglets de feuille de calcul (en 1/1000 de la largeur de la fenêtre). |
| [GetShowTabs](./getshowtabs/) | Obtient ou définit une valeur indiquant si les onglets du classeur sont affichés. |
| [SetShowTabs](./setshowtabs/) | Obtient ou définit une valeur indiquant si les onglets du classeur sont affichés. |
| [GetFirstVisibleTab](./getfirstvisibletab/) | Obtient ou définit le premier onglet de feuille de calcul visible. |
| [SetFirstVisibleTab](./setfirstvisibletab/) | Obtient ou définit le premier onglet de feuille de calcul visible. |
| [IsHScrollBarVisible](./ishscrollbarvisible/) | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale. |
| [SetIsHScrollBarVisible](./setishscrollbarvisible/) | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement horizontale. |
| [IsVScrollBarVisible](./isvscrollbarvisible/) | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale. |
| [SetIsVScrollBarVisible](./setisvscrollbarvisible/) | Obtient ou définit une valeur indiquant si la feuille de calcul générée contiendra une barre de défilement verticale. |
| [GetShared](./getshared/) | Obtient ou définit une valeur indiquant si le classeur est partagé. |
| [SetShared](./setshared/) | Obtient ou définit une valeur indiquant si le classeur est partagé. |
| [GetLanguageCode](./getlanguagecode/) | Obtient ou définit la langue de l'interface utilisateur de la version du Workbook basée sur le CountryCode du fichier enregistré. |
| [SetLanguageCode](./setlanguagecode/) | Obtient ou définit la langue de l'interface utilisateur de la version du Workbook basée sur le CountryCode du fichier enregistré. |
| [GetRegion](./getregion/) | Obtient ou définit les paramètres régionaux du classeur. |
| [SetRegion](./setregion/) | Obtient ou définit les paramètres régionaux du classeur. |
| [GetGlobalizationSettings](./getglobalizationsettings/) | Obtient et définit les paramètres de mondialisation. |
| [SetGlobalizationSettings](./setglobalizationsettings/) | Obtient et définit les paramètres de mondialisation. |
| [GetNumberDecimalSeparator](./getnumberdecimalseparator/) | Obtient ou définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle. |
| [SetNumberDecimalSeparator](./setnumberdecimalseparator/) | Obtient ou définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle. |
| [GetNumberGroupSeparator](./getnumbergroupseparator/) | Obtient ou définit le caractère qui sépare les groupes de chiffres à gauche du séparateur décimal dans les valeurs numériques. La valeur par défaut est le séparateur de groupe de la région actuelle. |
| [SetNumberGroupSeparator](./setnumbergroupseparator/) | Obtient ou définit le caractère qui sépare les groupes de chiffres à gauche du séparateur décimal dans les valeurs numériques. La valeur par défaut est le séparateur de groupe de la région actuelle. |
| [GetPassword](./getpassword/) | Représente le mot de passe de chiffrement du fichier du classeur. |
| [SetPassword](./setpassword/) | Représente le mot de passe de chiffrement du fichier du classeur. |
| [GetWriteProtection](./getwriteprotection/) | Fournit l'accès aux options de protection en écriture du classeur. |
| [IsEncrypted](./isencrypted/) | Obtient une valeur qui indique si un mot de passe est requis pour ouvrir ce classeur. |
| [IsProtected](./isprotected/) | Obtient une valeur qui indique si la structure ou la fenêtre du classeur est protégée. |
| [IsDefaultEncrypted](./isdefaultencrypted/) | Indique si le classeur doit être chiffré avec le mot de passe par défaut lorsque la structure et les fenêtres du classeur sont verrouillées. |
| [SetIsDefaultEncrypted](./setisdefaultencrypted/) | Indique si le classeur doit être chiffré avec le mot de passe par défaut lorsque la structure et les fenêtres du classeur sont verrouillées. |
| [IsMinimized](./isminimized/) | Représente si la feuille de calcul générée sera ouverte minimisée. |
| [SetIsMinimized](./setisminimized/) | Représente si la feuille de calcul générée sera ouverte minimisée. |
| [IsHidden](./ishidden/) | Indique si ce classeur est masqué. |
| [SetIsHidden](./setishidden/) | Indique si ce classeur est masqué. |
| [GetAutoCompressPictures](./getautocompresspictures/) | Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur. |
| [SetAutoCompressPictures](./setautocompresspictures/) | Spécifie une valeur booléenne qui indique que l'application compresse automatiquement les images dans le classeur. |
| [GetRemovePersonalInformation](./getremovepersonalinformation/) | Vrai si les informations personnelles peuvent être supprimées du classeur spécifié. |
| [SetRemovePersonalInformation](./setremovepersonalinformation/) | Vrai si les informations personnelles peuvent être supprimées du classeur spécifié. |
| [GetShapeDisplayType](./getshapedisplaytype/) | Obtient et définit comment l'application affiche les formes dans ce classeur. |
| [SetShapeDisplayType](./setshapedisplaytype/) | Obtient et définit comment l'application affiche les formes dans ce classeur. |
| [GetHidePivotFieldList](./gethidepivotfieldlist/) | Obtient et définit si la liste des champs du tableau croisé dynamique est masquée. |
| [SetHidePivotFieldList](./sethidepivotfieldlist/) | Obtient et définit si la liste des champs du tableau croisé dynamique est masquée. |
| [GetMaxUniqueItemsPerField](./getmaxuniqueitemsperfield/) | Obtient et définit la limitation du nombre d'éléments uniques par champ. |
| [SetMaxUniqueItemsPerField](./setmaxuniqueitemsperfield/) | Obtient et définit la limitation du nombre d'éléments uniques par champ. |
| [GetUpdateLinksType](./getupdatelinkstype/) | Obtient et définit comment les liens externes sont mis à jour lorsque le classeur est ouvert. |
| [SetUpdateLinksType](./setupdatelinkstype/) | Obtient et définit comment les liens externes sont mis à jour lorsque le classeur est ouvert. |
| [SetPageOrientationType](./setpageorientationtype/) | Définit le type d'orientation d'impression pour l'ensemble du classeur. |
| [GetMaxRow](./getmaxrow/) | Obtient l'index maximal de ligne, basé sur zéro. |
| [GetMaxColumn](./getmaxcolumn/) | Obtient l'index maximal de colonne, basé sur zéro. |
| [GetSmartTagOptions](./getsmarttagoptions/) | Obtient les options de la balise intelligente. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Obtient les paramètres des valeurs par défaut des propriétés liées au style pour ce classeur. |
| [GetWindowLeft](./getwindowleft/) | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en points. |
| [SetWindowLeft](./setwindowleft/) | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en points. |
| [GetWindowLeftInch](./getwindowleftinch/) | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en pouces. |
| [SetWindowLeftInch](./setwindowleftinch/) | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en pouces. |
| [GetWindowLeftCM](./getwindowleftcm/) | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en centimètres. |
| [SetWindowLeftCM](./setwindowleftcm/) | La distance du bord gauche de la zone client au bord gauche de la fenêtre, en centimètres. |
| [GetWindowTop](./getwindowtop/) | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en points. |
| [SetWindowTop](./setwindowtop/) | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en points. |
| [GetWindowTopInch](./getwindowtopinch/) | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en pouces. |
| [SetWindowTopInch](./setwindowtopinch/) | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en pouces. |
| [GetWindowTopCM](./getwindowtopcm/) | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en centimètres. |
| [SetWindowTopCM](./setwindowtopcm/) | La distance du bord supérieur de la zone client au bord supérieur de la fenêtre, en centimètres. |
| [GetWindowWidth](./getwindowwidth/) | La largeur de la fenêtre, en points. |
| [SetWindowWidth](./setwindowwidth/) | La largeur de la fenêtre, en points. |
| [GetWindowWidthInch](./getwindowwidthinch/) | La largeur de la fenêtre, en pouces. |
| [SetWindowWidthInch](./setwindowwidthinch/) | La largeur de la fenêtre, en pouces. |
| [GetWindowWidthCM](./getwindowwidthcm/) | La largeur de la fenêtre, en centimètres. |
| [SetWindowWidthCM](./setwindowwidthcm/) | La largeur de la fenêtre, en centimètres. |
| [GetWindowHeight](./getwindowheight/) | La hauteur de la fenêtre, en unité de point. |
| [SetWindowHeight](./setwindowheight/) | La hauteur de la fenêtre, en unité de point. |
| [GetWindowHeightInch](./getwindowheightinch/) | La hauteur de la fenêtre, en unité de pouce. |
| [SetWindowHeightInch](./setwindowheightinch/) | La hauteur de la fenêtre, en unité de pouce. |
| [GetWindowHeightCM](./getwindowheightcm/) | La hauteur de la fenêtre, en unité de centimètre. |
| [SetWindowHeightCM](./setwindowheightcm/) | La hauteur de la fenêtre, en unité de centimètre. |
| [GetUpdateAdjacentCellsBorder](./getupdateadjacentcellsborder/) | Indique si la bordure des cellules adjacentes doit être mise à jour. |
| [SetUpdateAdjacentCellsBorder](./setupdateadjacentcellsborder/) | Indique si la bordure des cellules adjacentes doit être mise à jour. |
| [GetSignificantDigitsType](./getsignificantdigitstype/) | Obtient et définit le type de chiffres significatifs pour la sortie des valeurs numériques dans ce classeur. La valeur par défaut est CellsHelper.SignificantDigitsType. |
| [SetSignificantDigitsType](./setsignificantdigitstype/) | Obtient et définit le type de chiffres significatifs pour la sortie des valeurs numériques dans ce classeur. La valeur par défaut est CellsHelper.SignificantDigitsType. |
| [GetCheckCompatibility](./getcheckcompatibility/) | Indique si la compatibilité avec les versions antérieures doit être vérifiée lors de l'enregistrement du classeur. |
| [SetCheckCompatibility](./setcheckcompatibility/) | Indique si la compatibilité avec les versions antérieures doit être vérifiée lors de l'enregistrement du classeur. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Indique si la restriction du fichier excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier excel, vous ne devez pas enregistrer le workbook au format excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier excel généré. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Indique si la restriction du fichier excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier excel, vous ne devez pas enregistrer le workbook au format excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier excel généré. |
| [GetAutoRecover](./getautorecover/) | Indique si le fichier est marqué pour la récupération automatique. |
| [SetAutoRecover](./setautorecover/) | Indique si le fichier est marqué pour la récupération automatique. |
| [GetCrashSave](./getcrashsave/) | indique si l'application a enregistré le fichier du classeur après un plantage. |
| [SetCrashSave](./setcrashsave/) | indique si l'application a enregistré le fichier du classeur après un plantage. |
| [GetDataExtractLoad](./getdataextractload/) | indique si l'application a ouvert le classeur pour la récupération de données. |
| [SetDataExtractLoad](./setdataextractload/) | indique si l'application a ouvert le classeur pour la récupération de données. |
| [GetRepairLoad](./getrepairload/) | Indique si l'application a ouvert le classeur en mode sécurisé ou de réparation. |
| [SetRepairLoad](./setrepairload/) | Indique si l'application a ouvert le classeur en mode sécurisé ou de réparation. |
| [GetBuildVersion](./getbuildversion/) | Spécifie la version publique incrémentielle de l'application. |
| [SetBuildVersion](./setbuildversion/) | Spécifie la version publique incrémentielle de l'application. |
| [GetMemorySetting](./getmemorysetting/) | Obtient ou définit les options d'utilisation de la mémoire. La nouvelle option sera prise comme option par défaut pour les feuilles de calcul nouvellement créées mais ne prendra pas effet pour les feuilles existantes. |
| [SetMemorySetting](./setmemorysetting/) | Obtient ou définit les options d'utilisation de la mémoire. La nouvelle option sera prise comme option par défaut pour les feuilles de calcul nouvellement créées mais ne prendra pas effet pour les feuilles existantes. |
| [GetPaperSize](./getpapersize/) | Obtient et définit la taille de papier d'impression par défaut. |
| [SetPaperSize](./setpapersize/) | Obtient et définit la taille de papier d'impression par défaut. |
| [GetMaxRowsOfSharedFormula](./getmaxrowsofsharedformula/) | Obtient et définit le nombre maximal de lignes pour la formule partagée. |
| [SetMaxRowsOfSharedFormula](./setmaxrowsofsharedformula/) | Obtient et définit le nombre maximal de lignes pour la formule partagée. |
| [GetCompliance](./getcompliance/) | Spécifie la version OOXML pour le document de sortie. La valeur par défaut est Ecma376_2006. |
| [SetCompliance](./setcompliance/) | Spécifie la version OOXML pour le document de sortie. La valeur par défaut est Ecma376_2006. |
| [GetQuotePrefixToStyle](./getquoteprefixtostyle/) | Indique si la définition de la propriété Style.QuotePrefix lors de la saisie de la valeur chaîne (qui commence par une apostrophe) dans la cellule |
| [SetQuotePrefixToStyle](./setquoteprefixtostyle/) | Indique si la définition de la propriété Style.QuotePrefix lors de la saisie de la valeur chaîne (qui commence par une apostrophe) dans la cellule |
| [GetFormulaSettings](./getformulasettings/) | Obtient les paramètres des fonctionnalités liées aux formules. |
| [GetPropertiesFollowChartPoint](./getpropertiesfollowchartpoint/) | Indique si les propriétés des points de données et les étiquettes de données dans tous les graphiques de ce classeur suivent leur référence. |
| [SetPropertiesFollowChartPoint](./setpropertiesfollowchartpoint/) | Indique si les propriétés des points de données et les étiquettes de données dans tous les graphiques de ce classeur suivent leur référence. |
| [GetDiscardImageEditData](./getdiscardimageeditdata/) | Indique si les données d'image en cours d'édition sont abandonnées. |
| [SetDiscardImageEditData](./setdiscardimageeditdata/) | Indique si les données d'image en cours d'édition sont abandonnées. |
| [GetDefaultImageResolution](./getdefaultimageresolution/) | Obtient et définit la résolution par défaut de l'image. |
| [SetDefaultImageResolution](./setdefaultimageresolution/) | Obtient et définit la résolution par défaut de l'image. |
| [GetWpsCompatibility](./getwpscompatibility/) | Indique si la compatibilité avec WPS doit être assurée. |
| [SetWpsCompatibility](./setwpscompatibility/) | Indique si la compatibilité avec WPS doit être assurée. |
