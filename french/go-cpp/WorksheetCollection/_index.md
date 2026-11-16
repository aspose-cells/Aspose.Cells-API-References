---
title: "WorksheetCollection Classe"
linktitle: "WorksheetCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "WorksheetCollection classe. Encapsule l'objet qui représente worksheetcollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/worksheetcollection/
---

## WorksheetCollection class

Encapsule une collection d'objets <see cref=\"Worksheet\"/>.

```go

type WorksheetCollection struct  {
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
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Obtient la liste des volets de tâches. |
| [GetWebExtensions](./getwebextensions/) | Obtient la liste des volets de tâches. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Obtient la liste des auteurs de commentaires en fil. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | Indique si toutes les connexions doivent être actualisées à l'ouverture du fichier dans MS Excel. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | Indique si toutes les connexions doivent être actualisées à l'ouverture du fichier dans MS Excel. |
| [CreateRange](./createrange/) | Crée un objet Range à partir d'une adresse de la plage. |
| [CreateUnionRange](./createunionrange/) | Crée un objet Range à partir d'une adresse de la plage. |
| [GetNames](./getnames/) | Obtient la collection de tous les objets Name dans la feuille de calcul. |
| [Get_Int](./get_int/) | Obtient l'élément Worksheet à l'index spécifié. |
| [Get_String](./get_string/) | Obtient l'élément Worksheet avec le nom spécifié. |
| [GetSheetByCodeName](./getsheetbycodename/) | Obtient la feuille de calcul par le nom de code. |
| [GetActiveSheetName](./getactivesheetname/) | Représente le nom de la feuille de calcul active lorsque le classeur est ouvert. |
| [SetActiveSheetName](./setactivesheetname/) | Représente le nom de la feuille de calcul active lorsque le classeur est ouvert. |
| [GetActiveSheetIndex](./getactivesheetindex/) | Représente l'index de la feuille de calcul active lorsque le classeur est ouvert. |
| [SetActiveSheetIndex](./setactivesheetindex/) | Représente l'index de la feuille de calcul active lorsque le classeur est ouvert. |
| [SortNames](./sortnames/) | Trie les noms définis. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | Insérer une feuille de calcul. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Insérer une feuille de calcul. |
| [Add_SheetType](./add_sheettype/) | Ajoute une feuille de calcul à la collection. |
| [SwapSheet](./swapsheet/) | Échange les deux feuilles. |
| [Add](./add/) | Ajoute une feuille de calcul à la collection. |
| [Add_String](./add_string/) | Ajoute une feuille de calcul à la collection. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Ajoute une fonction d'add‑in au classeur |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Ajoute une fonction d'add‑in au classeur |
| [RemoveAt_String](./removeat_string/) | Supprime l'élément avec un nom spécifié. |
| [RemoveAt_Int](./removeat_int/) | Supprime l'élément à un index spécifié. |
| [Clear](./clear/) | Efface toutes les feuilles de calcul. |
| [AddCopy_String](./addcopy_string/) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [AddCopy_Int](./addcopy_int/) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Copier un groupe de feuilles de calcul. |
| [GetDxfs](./getdxfs/) | Obtient les enregistrements de mise en forme différentielle maîtres. |
| [GetRangeByName_String](./getrangebyname_string/) | Obtient l'objet Range par nom prédéfini. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Obtient le Range par nom prédéfini ou par le nom de la table |
| [GetNamedRanges](./getnamedranges/) | Obtient toutes les plages nommées prédéfinies dans la feuille de calcul. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | Obtient toutes les plages nommées prédéfinies dans la feuille de calcul. |
| [GetXmlMaps](./getxmlmaps/) | Obtient et définit les cartes XML dans le classeur. |
| [SetXmlMaps](./setxmlmaps/) | Obtient et définit les cartes XML dans le classeur. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Renvoie une collection DocumentProperty qui représente toutes les propriétés de document intégrées de la feuille de calcul. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Renvoie une collection DocumentProperty qui représente toutes les propriétés de document personnalisées de la feuille de calcul. |
| [GetOleSize](./getolesize/) | Obtient et définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole. |
| [SetOleSize_Object](./setolesize_object/) | Obtient et définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole. |
| [GetExternalLinks](./getexternallinks/) | Représente les liens externes dans un classeur. |
| [GetPivotCaches](./getpivotcaches/) | Obtient tous les PivotCache. |
| [GetTableStyles](./gettablestyles/) | Obtient l'objet TableStyles. |
| [ClearPivottables](./clearpivottables/) | Efface les tableaux croisés dynamiques de la feuille de calcul. |
| [GetRevisionLogs](./getrevisionlogs/) | Représente les journaux de révision. |
| [RefreshPivotTables](./refreshpivottables/) | Actualise tous les PivotTables dans le fichier Excel. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Actualise tous les PivotTables dans le fichier Excel. |
| [GetSensitivityLabels](./getsensitivitylabels/) | Représente toutes les étiquettes de sensibilité. |
| [GetCount](./getcount/) | Obtient le nombre d'éléments contenus dans l'instance. |
