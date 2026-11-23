---
title: "Classe EbookLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.EbookLoadOptions. Représente les options lors de l'importation d'un fichier ebook"
type: docs
url: /fr/net/aspose.cells/ebookloadoptions/
---
## EbookLoadOptions class

Représente les options lors de l'importation d'un fichier ebook.

```csharp
public class EbookLoadOptions : HtmlLoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [EbookLoadOptions](ebookloadoptions/#constructor)() | Crée une option pour charger le fichier ebook. |
| [EbookLoadOptions](ebookloadoptions/#constructor_1)(LoadFormat) | Crée une option de chargement du fichier ebook. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolète.**) Le répertoire où les fichiers joints seront enregistrés.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indique si le filtrage automatique des données lors du chargement des fichiers est activé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Indique si l'ajustement automatique des colonnes et des lignes. La valeur par défaut est false.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtient et définit les options d'ajustement automatique (Hérité de [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Vérifie si les données sont valides dans le fichier modèle. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date. La valeur par défaut est true.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolète.**) si vrai, convertir la chaîne en formule lorsque la valeur de chaîne commence par le caractère '=', la valeur par défaut est false.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques. La valeur par défaut est true.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtient les paramètres de style par défaut pour l'initialisation des styles du classeur (Hérité de [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Indique si les espaces redondants sont supprimés lorsque le texte passe à la ligne en utilisant la balise `<br>`. La valeur par défaut est false.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | Indique s'il faut détecter les formules LaTeX dans le fichier HTML. La valeur par défaut est false.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Obtient et définit l'encodage par défaut. S'applique uniquement aux fichiers csv.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtient et définit les configurations de police individuelles. Ne fonctionne que pour le [`Workbook`](../workbook/) qui utilise ce [`LoadOptions`](../loadoptions/) pour le chargement. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Indique si le texte est une formule s'il commence par \"=\".(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | Spécifie comment les hyperliens sont chargés lors du chargement du HTML.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier (Hérité de [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indique s'il faut ignorer les formes inutiles. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtient et définit le moniteur d'interruption. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indique s'il ne faut pas analyser une valeur de chaîne si sa longueur est de 15.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indique s'il faut conserver les données non analysées en mémoire pour le classeur lorsqu'il est chargé à partir d'un fichier modèle. La valeur par défaut est vraie. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Le filtre indiquant comment charger les données. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtient le format de chargement. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Indique s'il faut importer les formules si le fichier html original contient des formules(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une valeur chaîne en nombre ou date/heure.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtient ou définit le mode mémoire pour le classeur chargé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolète.**) Spécifie comment les éléments HTML &lt;p&gt; sont rendus lors du chargement du HTML. La valeur par défaut est Normal.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | Spécifie comment les éléments HTML &lt;p&gt; sont rendus lors du chargement du HTML. La valeur par défaut est Normal.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indique s'il faut analyser la formule lors de la lecture du fichier. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indique s'il faut analyser les enregistrements en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtient et définit le mot de passe du classeur. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indique si l'on doit préserver ces espaces et sauts de ligne qui sont remplis entre les jetons de formule lors de la récupération et de la définition des formules. La valeur par défaut est false.(Hérité de [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Obtient l'identifiant du programme de création du fichier. Seulement pour les fichiers MHT.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Définit le nom de police standard par défaut (Hérité de [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Définit la taille de police standard par défaut. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Obtient ou définit le StreamProviderImportHtmlFile pour l'importation d'objets.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Indique si la mise en page de la balise `<div>` est prise en charge lorsque le fichier html la contient. La valeur par défaut est false.(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Obtenez l'instance de HtmlTableLoadOptionCollection(Hérité de [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement. (Hérité de [`LoadOptions`](../loadoptions/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Définit la taille de papier d'impression par défaut à partir des paramètres de l'imprimante par défaut. (Hérité de [`LoadOptions`](../loadoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;
    using System.Text;

    public class EbookLoadOptionsDemo
    {
        public static void EbookLoadOptionsExample()
        {
            // Créez une instance de EbookLoadOptions
            EbookLoadOptions options = new EbookLoadOptions();

            // Définition des propriétés
            options.AttachedFilesDirectory = "C:\\AttachedFiles";
            options.LoadFormulas = true;
            options.SupportDivTag = true;
            options.DeleteRedundantSpaces = true;
            options.AutoFitColsAndRows = true;
            options.ConvertFormulasData = true;
            options.HasFormula = true;
            options.Encoding = Encoding.UTF8;
            options.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            options.ConvertNumericData = true;
            options.ConvertDateTimeData = true;
            options.KeepPrecision = true;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = true;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
            options.StandardFontSize = 12.0;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter();
            options.LightCellsDataHandler = null; // Assuming no light cells data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = new IndividualFontConfigs();
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = true;

            // Chargez un fichier ebook dans un classeur en utilisant les options spécifiées
            Workbook workbook = new Workbook("EbookLoadOptionsExample_original.ebook", options);

            // Enregistrez le classeur dans un fichier Excel
            workbook.Save("EbookLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../htmlloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


