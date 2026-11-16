---
title: "Workbook Classe"
linktitle: "Workbook"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Workbook classe. Encapsule l'objet qui représente workbook en Go."
type: docs
weight: 200
url: /fr/go-cpp/workbook/
---

## Workbook class

Représente un objet racine pour créer une feuille de calcul Excel.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewWorkbook](./newworkbook/) | Initialise une nouvelle instance de la classe Workbook. |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Initialise une nouvelle instance de la classe Workbook. |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | Initialise une nouvelle instance vide de la classe Workbook avec des options |
| [NewWorkbook_String](./newworkbook_string/) | Initialise une nouvelle instance de la classe Workbook et ouvre un fichier. |
| [NewWorkbook_Stream](./newworkbook_stream/) | Initialise une nouvelle instance de la classe Workbook et ouvre un flux. |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Initialise une nouvelle instance de la classe Workbook et ouvre un fichier. |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | Initialise une nouvelle instance de la classe Workbook et ouvre le flux. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetSettings](./getsettings/) | Représente les paramètres du workbook. |
| [ParseFormulas](./parseformulas/) | Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées depuis le fichier modèle ou affectées à une cellule. |
| [StartAccessCache](./startaccesscache/) | Démarre la session qui utilise des caches pour accéder aux données. |
| [CloseAccessCache](./closeaccesscache/) | Ferme la session qui utilise des caches pour accéder aux données. |
| [Save_String_SaveFormat](./save_string_saveformat/) | Enregistre le classeur sur le disque. |
| [Save_String](./save_string/) | Enregistrez le classeur sur le disque. |
| [Save_String_SaveOptions](./save_string_saveoptions/) | Enregistre le classeur sur le disque. |
| [Save_SaveFormat](./save_saveformat/) | Enregistre le classeur dans le flux. |
| [Save_SaveOptions](./save_saveoptions/) | Enregistre le classeur dans le flux. |
| [SaveToStream](./savetostream/) | Enregistre le fichier Excel dans un objet MemoryStream au format Excel97-2003 xls et le renvoie. |
| [GetWorksheets](./getworksheets/) | Obtient la collection WorksheetCollection dans la feuille de calcul. |
| [IsLicensed](./islicensed/) | Indique si la licence est définie. |
| [RemoveUnusedStyles](./removeunusedstyles/) | Supprime tous les styles inutilisés. |
| [CreateStyle](./createstyle/) | Crée un nouveau style. |
| [CreateStyle_Bool](./createstyle_bool/) | Crée un nouveau style. |
| [CreateBuiltinStyle](./createbuiltinstyle/) | Crée un style intégré selon le type donné. |
| [CreateCellsColor](./createcellscolor/) | Crée un objet CellsColor. |
| [Replace_String_String](./replace_string_string/) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [Replace_String_Int](./replace_string_int/) | Remplace la valeur d'une cellule par un nouvel entier. |
| [Replace_String_Double](./replace_string_double/) | Remplace la valeur d'une cellule par un nouveau double. |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | Remplace la valeur d'une cellule par un nouveau tableau de chaînes. |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | Remplace les valeurs des cellules par un tableau d'entiers. |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | Remplace les valeurs des cellules par un tableau de doubles. |
| [Replace_Bool_Object](./replace_bool_object/) | Remplace les valeurs des cellules par de nouvelles données. |
| [Replace_Int_Object](./replace_int_object/) | Remplace les valeurs des cellules par de nouvelles données. |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | Remplace la valeur d'une cellule par une nouvelle chaîne. |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | Copie un autre objet Workbook. |
| [Copy_Workbook](./copy_workbook/) | Copie les données d'un objet Workbook source. |
| [Combine](./combine/) | Combine un autre objet Workbook. |
| [GetColors](./getcolors/) | Renvoie les couleurs de la palette pour la feuille de calcul. |
| [GetStyleInPool](./getstyleinpool/) | Obtient le style dans le pool de styles.Tous les styles du classeur seront rassemblés dans un pool.Il n'y a qu'un simple index de référence dans les cellules. |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | Obtient le nombre de styles dans le pool de styles. |
| [GetFonts](./getfonts/) | Obtient toutes les polices dans le pool de styles. |
| [GetNamedStyle](./getnamedstyle/) | Obtient le style nommé dans le pool de styles. |
| [MergeNamedStyles](./mergenamedstyles/) | Fusionne les styles nommés du autre fichier Excel. |
| [ChangePalette](./changepalette/) | Modifie la palette de la feuille de calcul à l'index spécifié. |
| [IsColorInPalette](./iscolorinpalette/) | Vérifie si une couleur se trouve dans la palette de la feuille de calcul. |
| [CalculateFormula](./calculateformula/) | Calcule le résultat des formules. |
| [CalculateFormula_Bool](./calculateformula_bool/) | Calcule le résultat des formules. |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | Calcul des formules dans ce classeur. |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines selon les données actuelles) Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules de tableau dynamique. |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines selon les données actuelles) |
| [GetDefaultStyle](./getdefaultstyle/) | Obtient ou définit l'objet Style par défaut du classeur. |
| [SetDefaultStyle](./setdefaultstyle/) | Obtient ou définit l'objet Style par défaut du classeur. |
| [GetMatchingColor](./getmatchingcolor/) | Trouve la couleur la plus proche dans la palette actuelle. |
| [IsDigitallySigned](./isdigitallysigned/) | Indique si cette feuille de calcul est signée numériquement. |
| [SetEncryptionOptions](./setencryptionoptions/) | Définit les options de chiffrement. |
| [Protect](./protect/) | Protège un classeur. |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | Protège un classeur partagé. |
| [Unprotect](./unprotect/) | Supprime la protection d'un classeur. |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Supprime la protection d'un classeur partagé. |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Indique si la structure ou la fenêtre est protégée par mot de passe. |
| [RemoveMacro](./removemacro/) | Supprime le VBA/macro de cette feuille de calcul. |
| [GetVbaProject](./getvbaproject/) | Obtient le VbaProject d'une feuille de calcul. |
| [RemoveDigitalSignature](./removedigitalsignature/) | Supprime la signature numérique de cette feuille de calcul. |
| [AcceptAllRevisions](./acceptallrevisions/) | Accepte toutes les modifications suivies dans le classeur. |
| [GetHasMacro](./gethasmacro/) | Indique si cette feuille de calcul contient des macros/VBA. |
| [GetHasRevisions](./gethasrevisions/) | Obtient si le classeur possède des modifications suivies. |
| [GetFileName](./getfilename/) | Obtient et définit le nom de fichier actuel. |
| [SetFileName](./setfilename/) | Obtient et définit le nom de fichier actuel. |
| [GetDataSorter](./getdatasorter/) | Obtient un objet DataSorter pour trier les données. |
| [GetThemeColor](./getthemecolor/) | Obtient la couleur du thème. |
| [SetThemeColor](./setthemecolor/) | Définit la couleur du thème |
| [GetTheme](./gettheme/) | Obtient le nom du thème. |
| [CustomTheme](./customtheme/) | Personnalise le thème. |
| [CopyTheme](./copytheme/) | Copie le thème d'un autre classeur. |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Met à jour la définition des fonctions personnalisées. |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | Si ce classeur contient des liens externes vers d'autres sources de données, Aspose.Cells tentera de récupérer les dernières données des sources fournies. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Renvoie une collection DocumentProperty qui représente toutes les propriétés de document intégrées de la feuille de calcul. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Renvoie une collection DocumentProperty qui représente toutes les propriétés de document personnalisées de la feuille de calcul. |
| [GetFileFormat](./getfileformat/) | Obtient et définit le format du fichier. |
| [SetFileFormat](./setfileformat/) | Obtient et définit le format du fichier. |
| [GetHasCustomFunction](./gethascustomfunction/) | Détecte si une fonction personnalisée est utilisée dans ce classeur, comme dans la formule d'une cellule, dans les noms définis... |
| [GetInterruptMonitor](./getinterruptmonitor/) | Obtient et définit le moniteur d'interruption. |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | Obtient et définit le moniteur d'interruption. |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | Définit le moniteur d'interruption. |
| [GetContentTypeProperties](./getcontenttypeproperties/) | Obtient la liste des objets ContentTypeProperty du classeur. |
| [GetCustomXmlParts](./getcustomxmlparts/) | Représente une partie de stockage de données XML personnalisées (données XML personnalisées au sein d'un package). |
| [GetDataMashup](./getdatamashup/) | Obtient les données mashup. |
| [GetRibbonXml](./getribbonxml/) | Obtient et définit le fichier XML qui définit l'interface du ruban. |
| [SetRibbonXml](./setribbonxml/) | Obtient et définit le fichier XML qui définit l'interface du ruban. |
| [GetAbsolutePath](./getabsolutepath/) | Obtient et définit le chemin absolu du fichier. |
| [SetAbsolutePath](./setabsolutepath/) | Obtient et définit le chemin absolu du fichier. |
| [GetDataConnections](./getdataconnections/) | Obtient la collection ExternalConnection. |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | Importe/Met à jour un fichier de données XML dans le classeur. |
| [ExportXml_String_String](./exportxml_string_string/) | Exporte les données XML liées par la carte XML spécifiée. |
| [ExportXml_String](./exportxml_string/) | Exporte les données XML. |
| [SetDigitalSignature](./setdigitalsignature/) | Définit la signature numérique d'un fichier de feuille de calcul (Excel2007 et versions ultérieures). |
| [AddDigitalSignature](./adddigitalsignature/) | Ajoute une signature numérique à un fichier de feuille de calcul OOXML (Excel2007 et versions ultérieures). |
| [GetDigitalSignature](./getdigitalsignature/) | Obtient la signature numérique du fichier. |
| [RemovePersonalInformation](./removepersonalinformation/) | Supprime les informations personnelles. |
| [GetDataModel](./getdatamodel/) | Obtient le modèle de données du classeur. |
| [RefreshAll](./refreshall/) | Actualiser les formes liées, tous les tableaux croisés dynamiques et les graphiques avec la source pivot. |
| [Dispose](./dispose/) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
