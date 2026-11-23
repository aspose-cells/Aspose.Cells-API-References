---
title: "WebCells.SetBorders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WebCells. Définit les bordures pour une plage de cellules"
type: docs
url: /fr/net/aspose.cells.gridweb.data/webcells/setborders/
---
## WebCells.SetBorders method

Définit les bordures d'une plage de cellules.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Le numéro de la première ligne de la plage (indexé à zéro). |
| firstColumn | Int32 | Le numéro de la première colonne de la plage (indexé à zéro). |
| rowNumber | Int32 | Le nombre de lignes. |
| columnNumber | Int32 | Le nombre de colonnes. |
| position | SetBorderPosition | La position de la bordure. |
| borderStyle | WebBorderStyle | Le style de bordure. |

### Exemples

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Voir aussi

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


