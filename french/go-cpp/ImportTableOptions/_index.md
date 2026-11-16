---
title: "Classe ImportTableOptions"
linktitle: "ImportTableOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ImportTableOptions class. Encapsule l'objet qui représente importtableoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/importtableoptions/
---

## ImportTableOptions class

Représente les options d'importation de données dans les cellules.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | Crée les options d'importation par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetConvertGridStyle](./getconvertgridstyle/) | Indique si le style de la vue grille doit être appliqué aux cellules. |
| [SetConvertGridStyle](./setconvertgridstyle/) | Indique si le style de la vue grille doit être appliqué aux cellules. |
| [GetConvertNumericData](./getconvertnumericdata/) | Obtient ou définit une valeur qui indique si la valeur chaîne doit être convertie en valeur numérique ou date. |
| [SetConvertNumericData](./setconvertnumericdata/) | Obtient ou définit une valeur qui indique si la valeur chaîne doit être convertie en valeur numérique ou date. |
| [GetInsertRows](./getinsertrows/) | Indique si de nouvelles lignes doivent être ajoutées lors de l'importation des enregistrements de données. |
| [SetInsertRows](./setinsertrows/) | Indique si de nouvelles lignes doivent être ajoutées lors de l'importation des enregistrements de données. |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | Indique si le déplacement de la première ligne vers le bas lors de l'insertion de lignes est activé. |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | Indique si le déplacement de la première ligne vers le bas lors de l'insertion de lignes est activé. |
| [IsFieldNameShown](./isfieldnameshown/) | Indique si le nom du champ doit être importé. |
| [SetIsFieldNameShown](./setisfieldnameshown/) | Indique si le nom du champ doit être importé. |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | Indique si la légende doit être exportée en tant que nom de champ |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | Indique si la légende doit être exportée en tant que nom de champ |
| [GetDateFormat](./getdateformat/) | Obtient ou définit la chaîne de format de date pour les cellules contenant des valeurs datetime importées. |
| [SetDateFormat](./setdateformat/) | Obtient ou définit la chaîne de format de date pour les cellules contenant des valeurs datetime importées. |
| [GetNumberFormats](./getnumberformats/) | Obtient ou définit les formats numériques |
| [SetNumberFormats](./setnumberformats/) | Obtient ou définit les formats numériques |
| [GetStyles](./getstyles/) | Obtient et définit les styles pour chaque colonne du tableau. |
| [SetStyles](./setstyles/) | Obtient et définit les styles pour chaque colonne du tableau. |
| [GetIsFormulas](./getisformulas/) | Indique si les données sont des formules. |
| [SetIsFormulas](./setisformulas/) | Indique si les données sont des formules. |
| [GetTotalRows](./gettotalrows/) | Obtient ou définit le nombre total de lignes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [SetTotalRows](./settotalrows/) | Obtient ou définit le nombre total de lignes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [GetTotalColumns](./gettotalcolumns/) | Obtient ou définit le nombre total de colonnes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [SetTotalColumns](./settotalcolumns/) | Obtient ou définit le nombre total de colonnes à importer depuis la source de données. -1 signifie toutes les lignes de la source de données donnée. |
| [GetColumnIndexes](./getcolumnindexes/) | Obtient ou définit les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées. |
| [SetColumnIndexes](./setcolumnindexes/) | Obtient ou définit les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées. |
| [GetDefaultValues](./getdefaultvalues/) | La valeur par défaut pour la valeur dans le tableau est null. |
| [SetDefaultValues](./setdefaultvalues/) | La valeur par défaut pour la valeur dans le tableau est null. |
| [IsHtmlString](./ishtmlstring/) | Indique si la valeur contient des balises html. |
| [SetIsHtmlString](./setishtmlstring/) | Indique si la valeur contient des balises html. |
| [GetCheckMergedCells](./getcheckmergedcells/) | Indique si la vérification des cellules fusionnées est activée. |
| [SetCheckMergedCells](./setcheckmergedcells/) | Indique si la vérification des cellules fusionnées est activée. |
