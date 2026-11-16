---
title: "Classe TxtLoadOptions"
linktitle: "TxtLoadOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe TxtLoadOptions. Encapsule l'objet qui représente txtloadoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/txtloadoptions/
---

## TxtLoadOptions class

Représente les options de chargement d'un fichier texte.

```go

type TxtLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewTxtLoadOptions](./newtxtloadoptions/) | Crée les options de chargement du fichier texte. |
| [NewTxtLoadOptions_LoadFormat](./newtxtloadoptions_loadformat/) | Crée les options de chargement du fichier texte. |
| [NewTxtLoadOptions_AbstractTextLoadOptions](./newtxtloadoptions_abstracttextloadoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetSeparator](./getseparator/) | Obtient et définit le séparateur de caractères du fichier texte. |
| [SetSeparator](./setseparator/) | Obtient et définit le séparateur de caractères du fichier texte. |
| [GetSeparatorString](./getseparatorstring/) | Obtient et définit une valeur chaîne comme séparateur. |
| [SetSeparatorString](./setseparatorstring/) | Obtient et définit une valeur chaîne comme séparateur. |
| [IsMultiEncoded](./ismultiencoded/) | True signifie que le fichier contient plusieurs encodages. |
| [SetIsMultiEncoded](./setismultiencoded/) | True signifie que le fichier contient plusieurs encodages. |
| [GetHasFormula](./gethasformula/) | Indique si le texte est une formule s'il commence par "=","Obtient et définit l'encodage par défaut. S'applique uniquement aux fichiers csv. |
| [SetHasFormula](./sethasformula/) | Indique si le texte est une formule s'il commence par "=","Obtient et définit l'encodage par défaut. S'applique uniquement aux fichiers csv. |
| [GetHasTextQualifier](./gethastextqualifier/) | Indique s'il existe un qualificateur de texte pour la valeur de la cellule. La valeur par défaut est true. |
| [SetHasTextQualifier](./sethastextqualifier/) | Indique s'il existe un qualificateur de texte pour la valeur de la cellule. La valeur par défaut est true. |
| [GetTextQualifier](./gettextqualifier/) | Spécifie le qualificateur de texte pour les valeurs de cellule. Le qualificateur par défaut est '"'. |
| [SetTextQualifier](./settextqualifier/) | Spécifie le qualificateur de texte pour les valeurs de cellule. Le qualificateur par défaut est '"'. |
| [GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | Indique si les délimiteurs consécutifs doivent être traités comme un seul. |
| [SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | Indique si les délimiteurs consécutifs doivent être traités comme un seul. |
| [GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | Indique si le signe apostrophe simple initial doit être considéré comme faisant partie de la valeur d'une cellule. La valeur par défaut est true. Si elle est false, l'apostrophe simple initiale sera supprimée de la valeur de la cellule correspondante et Style.QuotePrefix sera défini sur true pour la cellule. |
| [SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | Indique si le signe apostrophe simple initial doit être considéré comme faisant partie de la valeur d'une cellule. La valeur par défaut est true. Si elle est false, l'apostrophe simple initiale sera supprimée de la valeur de la cellule correspondante et Style.QuotePrefix sera défini sur true pour la cellule. |
| [GetExtendToNextSheet](./getextendtonextsheet/) | Indique si les données sont étendues à la feuille suivante lorsque les lignes ou colonnes dépassent la limite. La valeur par défaut est false. |
| [SetExtendToNextSheet](./setextendtonextsheet/) | Indique si les données sont étendues à la feuille suivante lorsque les lignes ou colonnes dépassent la limite. La valeur par défaut est false. |
| [GetHeaderRowsCount](./getheaderrowscount/) | Le nombre de lignes d'en-tête à répéter pour les feuilles étendues. |
| [SetHeaderRowsCount](./setheaderrowscount/) | Le nombre de lignes d'en-tête à répéter pour les feuilles étendues. |
| [GetHeaderColumnsCount](./getheadercolumnscount/) | Le nombre de colonnes d'en-tête à répéter pour les feuilles étendues. |
| [SetHeaderColumnsCount](./setheadercolumnscount/) | Le nombre de colonnes d'en-tête à répéter pour les feuilles étendues. |
| [GetMaxRowCount](./getmaxrowcount/) | Le nombre maximal de lignes à importer pour une feuille. |
| [SetMaxRowCount](./setmaxrowcount/) | Le nombre maximal de lignes à importer pour une feuille. |
| [GetMaxColumnCount](./getmaxcolumncount/) | Le nombre maximal de colonnes à importer pour une feuille. |
| [SetMaxColumnCount](./setmaxcolumncount/) | Le nombre maximal de colonnes à importer pour une feuille. |
| [GetEncoding](./getencoding/) | Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure. |
| [SetEncoding](./setencoding/) | Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques. La valeur par défaut est true. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques. La valeur par défaut est true. |
| [GetConvertNumericData](./getconvertnumericdata/) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date. La valeur par défaut est true. |
| [SetConvertNumericData](./setconvertnumericdata/) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date. La valeur par défaut est true. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | Indique de ne pas analyser une valeur de chaîne si la longueur est de 15. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | Indique de ne pas analyser une valeur de chaîne si la longueur est de 15. |
| [GetKeepPrecision](./getkeepprecision/) | Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15. |
| [SetKeepPrecision](./setkeepprecision/) | Indique s'il ne faut pas analyser une valeur de chaîne si la longueur est de 15. |
| [GetLoadFormat](./getloadformat/) | Obtient le format de chargement. |
| [GetPassword](./getpassword/) | Obtient et définit le mot de passe du Workbook. |
| [SetPassword](./setpassword/) | Obtient et définit le mot de passe du Workbook. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Indique si la formule est analysée lors de la lecture du fichier. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Indique si la formule est analysée lors de la lecture du fichier. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. La valeur par défaut est false. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Indique si les enregistrements mis en cache du tableau croisé dynamique sont analysés lors du chargement du fichier. La valeur par défaut est false. |
| [SetPaperSize](./setpapersize/) | Définit la taille de papier d'impression par défaut à partir des paramètres de l'imprimante par défaut. |
| [GetLanguageCode](./getlanguagecode/) | Obtient ou définit la langue de l'interface utilisateur de la version du Workbook basée sur le CountryCode du fichier enregistré. |
| [SetLanguageCode](./setlanguagecode/) | Obtient ou définit la langue de l'interface utilisateur de la version du Workbook basée sur le CountryCode du fichier enregistré. |
| [GetRegion](./getregion/) | Obtient ou définit les paramètres régionaux utilisés pour le Workbook qui sera chargé. |
| [SetRegion](./setregion/) | Obtient ou définit les paramètres régionaux utilisés pour le Workbook qui sera chargé. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Obtient les paramètres de style par défaut pour l'initialisation des styles du Workbook. |
| [GetInterruptMonitor](./getinterruptmonitor/) | Obtient et définit le moniteur d'interruption. |
| [SetInterruptMonitor](./setinterruptmonitor/) | Obtient et définit le moniteur d'interruption. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier. |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier. |
| [GetCheckDataValid](./getcheckdatavalid/) | Vérifie si les données sont valides dans le fichier modèle. |
| [SetCheckDataValid](./setcheckdatavalid/) | Vérifie si les données sont valides dans le fichier modèle. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Indique si la restriction du fichier excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier excel, vous ne devez pas enregistrer le workbook au format excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier excel généré. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Indique si la restriction du fichier excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier excel, vous ne devez pas enregistrer le workbook au format excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier excel généré. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | Indique si les données non analysées sont conservées en mémoire pour le Workbook lorsqu'il est chargé depuis le fichier modèle. La valeur par défaut est true. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | Indique si les données non analysées sont conservées en mémoire pour le Workbook lorsqu'il est chargé depuis le fichier modèle. La valeur par défaut est true. |
| [GetLoadFilter](./getloadfilter/) | Le filtre indiquant comment charger les données. |
| [SetLoadFilter](./setloadfilter/) | Le filtre indiquant comment charger les données. |
| [GetMemorySetting](./getmemorysetting/) | Obtient ou définit le mode mémoire pour le workbook chargé. |
| [SetMemorySetting](./setmemorysetting/) | Obtient ou définit le mode mémoire pour le workbook chargé. |
| [GetAutoFitterOptions](./getautofitteroptions/) | Obtient et définit les options de l'ajustement automatique. |
| [SetAutoFitterOptions](./setautofitteroptions/) | Obtient et définit les options de l'ajustement automatique. |
| [GetAutoFilter](./getautofilter/) | Indique si le filtrage automatique des données est appliqué lors du chargement des fichiers. |
| [SetAutoFilter](./setautofilter/) | Indique si le filtrage automatique des données est appliqué lors du chargement des fichiers. |
| [GetFontConfigs](./getfontconfigs/) | Obtient et définit les configurations de police individuelles. Ne fonctionne que pour le Workbook qui utilise ces LoadOptions pour le chargement. |
| [SetFontConfigs](./setfontconfigs/) | Obtient et définit les configurations de police individuelles. Ne fonctionne que pour le Workbook qui utilise ces LoadOptions pour le chargement. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | Indique si les formes inutiles sont ignorées. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | Indique si les formes inutiles sont ignorées. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Indique si les espaces et sauts de ligne insérés entre les jetons de formule sont conservés lors de l'obtention et de la définition des formules. La valeur par défaut est false. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Indique si les espaces et sauts de ligne insérés entre les jetons de formule sont conservés lors de l'obtention et de la définition des formules. La valeur par défaut est false. |
