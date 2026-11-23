---
title: "Classe Workbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Workbook. Représente un objet racine pour créer une feuille de calcul Excel"
type: docs
url: /fr/net/aspose.cells/workbook/
---
## Workbook class

Représente un objet racine pour créer une feuille de calcul Excel.

```csharp
public class Workbook : IDisposable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Workbook](workbook/#constructor)() | Initialise une nouvelle instance de la classe `Workbook`. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | Initialise une nouvelle instance de la classe `Workbook`. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | Initialise une nouvelle instance vide de la classe `Workbook` avec des options |
| [Workbook](workbook/#constructor_3)(Stream) | Initialise une nouvelle instance de la classe `Workbook` et ouvre un flux. |
| [Workbook](workbook/#constructor_5)(string) | Initialise une nouvelle instance de la classe `Workbook` et ouvre un fichier. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | Initialise une nouvelle instance de la classe `Workbook` et ouvre le flux. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | Initialise une nouvelle instance de la classe `Workbook` et ouvre un fichier. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Obtient et définit le chemin absolu du fichier. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Renvoie une collection [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document intégrées du classeur. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Obtient la fabrique pour créer ICellsDataTable à partir d'objets personnalisés |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Renvoie les couleurs de la palette pour la feuille de calcul. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Obtient la liste des objets [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) dans le classeur. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Obtient le nombre de styles dans le pool de styles. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Renvoie une collection [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document personnalisées du classeur. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Représente une partie de stockage de données XML personnalisées (données XML personnalisées dans un package). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | Obtient la collection [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/). |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Obtient les données mashup. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Obtient le modèle de données dans le classeur. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Obtient un objet DataSorter pour trier les données. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Obtient ou définit l'objet [`Style`](../style/) par défaut du classeur. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Obtient et définit le format de fichier. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Obtient et définit le nom de fichier actuel. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Détecte s'il existe une fonction personnalisée utilisée dans ce classeur, comme dans la formule d'une cellule, dans les noms définis... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Indique si cette feuille de calcul contient des macros/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Obtient si le classeur possède des modifications suivies |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Obtient et définit le moniteur d'interruption. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Indique si cette feuille de calcul est signée numériquement. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Indique si la licence est définie. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Indique si la structure ou la fenêtre est protégée par mot de passe. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Obtient et définit le fichier XML qui définit l'interface Ribbon. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Représente les paramètres du classeur. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Obtient le nom du thème. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Obtient le [`VbaProject`](./vbaproject/) dans une feuille de calcul. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Obtient la collection [`WorksheetCollection`](../worksheetcollection/) dans la feuille de calcul. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Accepte toutes les modifications suivies dans le classeur. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | Ajoute une signature numérique à un fichier de feuille de calcul OOXML (Excel2007 et versions ultérieures). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Calcule le résultat des formules. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Calcule le résultat des formules. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Calcul des formules dans ce classeur. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Modifie la palette de la feuille de calcul à l'index spécifié. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Ferme la session qui utilise des caches pour accéder aux données. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Combine un autre objet Workbook. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Copie les données d'un objet Workbook source. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Copie un autre objet Workbook. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Copie le thème d'un autre classeur. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Crée un style intégré selon le type donné. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Crée un objet [`CellsColor`](../cellscolor/) . |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Crée un nouveau style. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Crée un nouveau style. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Personnalise le thème. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Effectue des tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | Exporte les données XML. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Exporte les données XML liées par la carte XML spécifiée. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Obtient la signature numérique du fichier. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Obtient toutes les polices dans le pool de styles. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Trouve la couleur correspondante la plus proche dans la palette actuelle. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Obtient le style nommé dans le pool de styles. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Obtient le style dans le pool de styles. Tous les styles du classeur seront rassemblés dans un pool. Il n'y a qu'un simple index de référence dans les cellules. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Obtient la couleur du thème. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolète.**) Indique si ce classeur contient des liens externes vers d'autres sources de données. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Vérifie si une couleur se trouve dans la palette de la feuille de calcul. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Fusionne les styles nommés du autre fichier Excel. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées depuis le fichier modèle ou affectées à une cellule. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Protège un classeur. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Protège un classeur partagé. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | Actualise les formes liées, tous les tableaux croisés dynamiques et les graphiques avec la source du tableau croisé dynamique. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Actualise les formules de tableau dynamique(débordent dans une nouvelle plage de cellules voisines selon les données actuelles) Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules de tableau dynamique. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Actualise les formules de tableau dynamique(débordent dans une nouvelle plage de cellules voisines selon les données actuelles) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Supprime la signature numérique de cette feuille de calcul. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolète.**) Supprime tous les liens externes du classeur. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Supprime le VBA/macro de cette feuille de calcul. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Supprime les informations personnelles. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Supprime tous les styles inutilisés. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Remplace les valeurs des cellules par de nouvelles données. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Remplace les valeurs des cellules par de nouvelles données. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Remplace les valeurs des cellules par des données provenant d'un DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Remplace la valeur d'une cellule par un nouveau double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Remplace la valeur d'une cellule par un nouvel entier. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Remplace les valeurs des cellules par un tableau de doubles. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Remplace les valeurs des cellules par un tableau d'entiers. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Remplace la valeur d'une cellule par un nouveau tableau de chaînes. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Enregistre le classeur sur le disque. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Enregistre le classeur dans le flux. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Enregistre le classeur dans le flux. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Enregistre le classeur sur le disque. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Enregistre le classeur sur le disque. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Crée la feuille de calcul résultante et la transfère au client, puis l'ouvre dans le navigateur ou le classeur MS. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Crée la feuille de calcul résultante et la transfère au client, puis l'ouvre dans le navigateur ou le classeur MS. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Enregistre le fichier Excel dans un objet MemoryStream en tant que fichier xls Excel97-2003 et le renvoie. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Applique une signature numérique à un fichier de feuille de calcul (Excel2007 et versions ultérieures). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Définir les options de chiffrement. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Définit la couleur du thème |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Démarre la session qui utilise des caches pour accéder aux données. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Supprime la protection d’un classeur. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Supprime la protection d’un classeur partagé. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Met à jour la définition des fonctions personnalisées. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | Si ce classeur contient des liens externes vers d’autres sources de données, Aspose.Cells tentera de récupérer les dernières données des sources fournies. |

### Remarques

La classe Workbook désigne une feuille de calcul Excel. Chaque feuille de calcul peut contenir plusieurs feuilles de calcul. La fonctionnalité de base de la classe est d’ouvrir et d’enregistrer des fichiers Excel natifs. La classe possède des fonctionnalités avancées comme la copie de données depuis d’autres Workbooks, la combinaison de deux Workbooks, la conversion d’Excel en PDF, le rendu d’Excel en image et la protection de la feuille de calcul Excel.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // Créer une nouvelle instance de Workbook
            Workbook workbook = new Workbook();

            // Accéder à la feuille de calcul par défaut
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir certaines propriétés du classeur
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Ajouter une nouvelle feuille de calcul
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Ajouter des données à la nouvelle feuille de calcul
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Définir certaines propriétés du document
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Enregistrer le classeur dans un fichier
            workbook.Save("WorkbookExample.xlsx");

            // Afficher certaines propriétés
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Vérifier si le classeur est sous licence
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Vérifier si le classeur est signé numériquement
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Vérifier si le classeur contient des macros
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Vérifier si le classeur possède des modifications suivies
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Vérifier le nombre de styles dans le pool de styles
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Vérifier le nom du thème
            Console.WriteLine("Theme: " + workbook.Theme);

            // Vérifier si le classeur est protégé par un mot de passe
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Vérifier si le classeur contient des liens externes
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // Libérer le classeur
            workbook.Dispose();
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


