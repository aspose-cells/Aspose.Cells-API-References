---
title: "PivotCache.SourceCellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotCache. Retourne la plage de la source de données utilisée avec SourceSheet."
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

Renvoie la plage de la source de données utilisée avec SourceSheet.

```csharp
public WebCellArea SourceCellArea { get; }
```

### Exemples

```csharp

 [C#]

 //Modifie la plage de la source de données
 //Valeur originale : StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //Ajoute des données de 2 lignes
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### Voir aussi

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


