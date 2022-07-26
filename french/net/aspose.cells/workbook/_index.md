---
title: Workbook
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente un objet racine pour créer une feuille de calcul Excel.
type: docs
weight: 6480
url: /fr/net/aspose.cells/workbook/
---
## Workbook class

Représente un objet racine pour créer une feuille de calcul Excel.

```csharp
public class Workbook : IDisposable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Workbook](workbook#constructor)() | Initialise une nouvelle instance du[`Workbook`](../workbook) classe. |
| [Workbook](workbook#constructor_1)(FileFormatType) | Initialise une nouvelle instance du[`Workbook`](../workbook) classe. |
| [Workbook](workbook#constructor_2)(Stream) | Initialise une nouvelle instance du[`Workbook`](../workbook) classe et ouvrez un flux. |
| [Workbook](workbook#constructor_4)(string) | Initialise une nouvelle instance du[`Workbook`](../workbook) classe et ouvrez un fichier. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | Initialise une nouvelle instance du[`Workbook`](../workbook) classe et flux ouvert. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | Initialise une nouvelle instance du[`Workbook`](../workbook) classe et ouvrez un fichier. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | Obtient et définit le chemin absolu du fichier. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | Renvoie un[`DocumentProperty`](../../aspose.cells.properties/documentproperty)collection qui représente toutes les propriétés de document intégrées de la feuille de calcul. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | Obtient la fabrique pour construire ICellsDataTable à partir d'objets personnalisés |
| [Colors](../../aspose.cells/workbook/colors) { get; } | Renvoie les couleurs dans la palette de la feuille de calcul. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | Obtient la liste des[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) objets dans le classeur. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | Obtient le nombre de styles dans le pool de styles. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | Renvoie un[`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection qui représente toutes les propriétés de document personnalisées de la feuille de calcul. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | Représente une partie de stockage de données XML personnalisée (données XML personnalisées dans un package). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | Obtient le[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) collection. |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | Obtient les données de mashup. |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | Obtient un objet DataSorter pour trier les données. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | Obtient ou définit la valeur par défaut[`Style`](../style) objet du classeur. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | Obtient et définit le format de fichier. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | Obtient et définit le nom du fichier actuel. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | Indique si cette feuille de calcul contient macro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | Obtient si le classeur contient des modifications suivies |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | Obtient et définit le moniteur d'interruption. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | Indique si cette feuille de calcul est signée numériquement. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | Indique si la licence est définie. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | Indique si la structure ou la fenêtre est protégée par mot de passe. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | Obtient et définit le fichier XML qui définit l'interface utilisateur du ruban. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | Représente les paramètres du classeur. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | Obtient le nom du thème. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | Obtient le[`VbaProject`](./vbaproject) dans une feuille de calcul. |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | Obtient le[`WorksheetCollection`](../worksheetcollection) collection dans la feuille de calcul. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | Accepte toutes les modifications suivies dans le classeur. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | Ajoute une signature numérique à un fichier de feuille de calcul OOXML (Excel2007 et versions ultérieures). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | Calcule le résultat des formules. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | Calcule le résultat des formules. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | Calcul des formules dans ce classeur. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | Modifie la palette de la feuille de calcul dans l'index spécifié. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | Ferme la session qui utilise des caches pour accéder aux données. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | Combine un autre objet Workbook. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | Copie les données d'un objet Workbook source. |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | Copie les données d'un objet Workbook source. |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | Copie le thème d'un autre classeur. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | Crée un style intégré par type donné. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | Crée un[`CellsColor`](../cellscolor) objet. |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | Crée un nouveau style. |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | Personnalise le thème. |
| [Dispose](../../aspose.cells/workbook/dispose)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | Exporter les données XML. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | Exporter les données XML liées par le mappage XML spécifié. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | Obtient la signature numérique du fichier. |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | Récupère toutes les polices du pool de styles. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | Trouver la meilleure couleur correspondante dans la palette actuelle. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | Obtient le style nommé dans le pool de styles. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | Obtient le style dans le pool de styles. Tous les styles du classeur seront rassemblés dans un pool. Il n'y a qu'un simple index de référence dans les cellules. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | Obtient la couleur du thème. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | Vérifie si une couleur est dans la palette de la feuille de calcul. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées à partir d'un fichier de modèle ou définies dans une cellule. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | Protège un classeur. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | Protège un classeur partagé. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | Actualise les formules de tableau dynamique (se répand dans une nouvelle plage de cellules voisines en fonction des données actuelles) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | Supprime la signature numérique de cette feuille de calcul. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | Supprime VBA/macro de cette feuille de calcul. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | Supprime les informations personnelles. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | Supprimer tous les styles inutilisés. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | Remplace les valeurs des cellules par de nouvelles données. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | Remplace les valeurs des cellules par de nouvelles données. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | Remplace les valeurs des cellules par les données d'unDataTable . |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | Remplace la valeur d'une cellule par un nouveau double. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | Remplace la valeur d'une cellule par un nouvel entier. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | Remplace les valeurs des cellules par un double tableau. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | Remplace les valeurs des cellules par un tableau d'entiers. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | Remplace la valeur d'une cellule par un nouveau tableau de chaînes. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | Enregistrez le classeur sur le disque. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | Enregistre le classeur dans le flux. |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | Enregistre le classeur dans le flux. |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | Enregistre le classeur sur le disque. |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | Enregistre le classeur sur le disque. |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Crée la feuille de calcul des résultats et la transfère au client, puis l'ouvre dans le navigateur ou MS Workbook. |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Crée la feuille de calcul des résultats et la transfère au client, puis l'ouvre dans le navigateur ou MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | Enregistre le fichier Excel dans un objet MemoryStream et le renvoie. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | Définit la signature numérique d'un fichier de feuille de calcul (Excel2007 et versions ultérieures). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | Définir les options de chiffrement. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | Définit la couleur du thème |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | Démarre la session qui utilise les caches pour accéder aux données. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | Déprotége un classeur. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | Déprotége un classeur partagé. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | Si ce classeur contient des liens externes vers d'autres sources de données, Aspose.Cells tentera de récupérer les dernières données. |

### Remarques

La classe Workbook désigne une feuille de calcul Excel. Chaque feuille de calcul peut contenir plusieurs feuilles de calcul. La fonctionnalité de base de la classe est d'ouvrir et d'enregistrer des fichiers Excel natifs. La classe possède des fonctionnalités avancées telles que la copie de données à partir d'autres classeurs, la combinaison de deux classeurs et la protection de la feuille de calcul Excel.

### Exemples

L'exemple suivant charge un classeur à partir d'un fichier nommé designer.xls et rend les barres de défilement horizontales et verticales invisibles pour le classeur. Il remplace ensuite deux valeurs de chaîne par une valeur entière et une valeur de chaîne respectivement dans la feuille de calcul et envoie enfin le fichier mis à jour au navigateur client.

```csharp
[C#]

//Ouvre un fichier de concepteur
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//Définir les barres de défilement
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//Remplacer la chaîne d'espace réservé par de nouvelles valeurs
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Ouvrir un fichier de concepteur
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Définir des barres de défilement
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Remplacer la chaîne d'espace réservé par de nouvelles valeurs
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
