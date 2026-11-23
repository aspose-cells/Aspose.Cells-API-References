---
title: "WebCells.Export"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WebCells. Exporte les données de la collection Cells d'une WebWorksheet vers un nouvel objet DataTable"
type: docs
url: /fr/net/aspose.cells.gridweb.data/webcells/export/
---
## WebCells.Export method

Exporte les données de la collection Cells d'un WebWorksheet vers un nouvel objet DataTable

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| exportColumnName | Boolean | Indique si les données de la première ligne sont exportées comme nom de colonne du DataTable |
| isVertical | Boolean | Vrai si une ligne du fichier Excel représente une ligne dans le DataTable. Faux si une colonne du fichier Excel représente une ligne dans le DataTable. |

### Valeur de retour

Objet DataTable exporté.

### Voir aussi

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


