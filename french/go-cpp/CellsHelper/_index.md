---
title: "Classe CellsHelper"
linktitle: "CellsHelper"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe CellsHelper. Encapsule l'objet qui représente cellshelper en Go."
type: docs
weight: 200
url: /fr/go-cpp/cellshelper/
---

## CellsHelper class

Fournit des fonctions d'assistance.

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | Obtient et définit le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. La valeur par défaut est SignificantDigitsType.G17. |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | Obtient et définit le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. La valeur par défaut est SignificantDigitsType.G17. |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | Obtient le DPI de la machine. |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | Obtient le DPI de la machine. |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | Obtient la largeur du texte en points. |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | Obtient la version de publication. |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | Obtient les index de ligne et de colonne de la cellule selon son nom. |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | Obtient le nom de la cellule selon ses index de ligne et de colonne. |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | Obtient le nom de la colonne selon l'index de colonne. |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | Obtient l'index de colonne selon le nom de colonne. |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | Obtient le nom de ligne selon l'index de ligne. |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | Obtient l'index de ligne selon le nom de ligne. |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | Convertit la valeur double en valeur date‑heure. |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | Convertit la date‑heure en valeur double. |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | Obtient ou définit le chemin de démarrage, qui est référencé par certaines références de formules externes. |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | Obtient ou définit le chemin de démarrage, qui est référencé par certaines références de formules externes. |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | Obtient ou définit le chemin de démarrage alternatif, qui est référencé par certaines références de formules externes. |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | Obtient ou définit le chemin de démarrage alternatif, qui est référencé par certaines références de formules externes. |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | Obtient ou définit le chemin de la bibliothèque qui est référencé par certaines références de formules externes. |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | Obtient ou définit le chemin de la bibliothèque qui est référencé par certaines références de formules externes. |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | Obtient toutes les couleurs utilisées dans le classeur. |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | Fusionne plusieurs gros fichiers xls en un fichier xls. |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | Obtient le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | Définit le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles des noms de feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si la longueur dépasse la limite et les caractères invalides seront remplacés par ' ', puis la valeur de chaîne reconstruite sera renvoyée. |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles des noms de feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si la longueur dépasse la limite et les caractères invalides seront remplacés par le caractère fourni, puis la valeur de chaîne reconstruite sera renvoyée. |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | Indique si le nom de la feuille doit être entouré de guillemets simples. |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc., |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc., |
