---
title: "LoadDataFilterOptions Enum"
linktitle: "LoadDataFilterOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "LoadDataFilterOptions enum. Encapsule l'objet qui représente loaddatafilteroptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/loaddatafilteroptions/
---

## LoadDataFilterOptions Enum

Représente les options de filtrage des données lors du chargement du classeur à partir d'un modèle.

```go

type LoadDataFilterOptions int32


```

## Champs

| Champ | Description |
| --- | --- |
| [All](./all/) | Tout charger |
| [CellBlank](./cellblank/) | Charger les cellules dont la valeur est vide |
| [CellString](./cellstring/) | Charger les cellules dont la valeur est une chaîne |
| [CellNumeric](./cellnumeric/) | Charger les cellules dont la valeur est numérique (incluant la date/heure) |
| [CellError](./cellerror/) | Charger les cellules dont la valeur est une erreur |
| [CellBool](./cellbool/) | Charger les cellules dont la valeur est booléenne |
| [CellValue](./cellvalue/) | Charger uniquement la valeur des cellules (tous les types de valeur) |
| [Formula](./formula/) | Charger les formules des cellules. |
| [CellData](./celldata/) | Charger les données des cellules, y compris les valeurs, les formules et le formatage |
| [Chart](./chart/) | Charger les graphiques |
| [Drawing](./drawing/) | Objets de dessin (incluant Chart, Picture, OleObject et tous les autres objets de dessin) |
| [MergedArea](./mergedarea/) | Charger les cellules fusionnées |
| [ConditionalFormatting](./conditionalformatting/) | Charger le formatage conditionnel |
| [DataValidation](./datavalidation/) | Charger les validations de données |
| [PivotTable](./pivottable/) | Charger les tableaux croisés dynamiques |
| [Table](./table/) | Charger les tableaux |
| [Hyperlinks](./hyperlinks/) | Charger les hyperliens |
| [SheetSettings](./sheetsettings/) | Charger les paramètres de la feuille de calcul |
| [SheetData](./sheetdata/) | Charger toutes les données de la feuille de calcul, telles que les données des cellules, les paramètres, les objets, ...etc. |
| [BookSettings](./booksettings/) | Charger les paramètres du classeur |
| [Settings](./settings/) | Charger les paramètres du classeur et de la feuille de calcul |
| [XmlMap](./xmlmap/) | Charger XmlMap |
| [Structure](./structure/) | Charger la structure du classeur |
| [Document_Properties](./document_properties/) | Charger les propriétés du document |
| [DefinedNames](./definednames/) | Charger les objets Name définis |
| [VBA](./vba/) | Charger les projets VBA |
| [Style](./style/) | Charger les styles pour le formatage des cellules |
| [Picture](./picture/) | Charger les images |
| [OleObject](./oleobject/) | Charger OleObjects |
| [Revision](./revision/) | Charger les journaux de révision |
