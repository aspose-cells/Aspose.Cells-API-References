---
title: "GridWorksheet.FilterString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridWorksheet méthode. Définit le filtre pour la colonne. Remarque : nous devons appeler AddAutoFilter avant d’appeler filterString. La chaîne de critères du filtre. Remarque : nous utilisons la virgule comme caractère de séparation, ainsi la valeur de cellule que vous souhaitez filtrer ne doit pas contenir de virgule. filterString10123456 signifie que la colonne 10 doit contenir 123 ou 456. filterString10123 signifie que la colonne 10 doit contenir 123. L’index de colonne est séparé par des virgules, ex. 123456789 ou abc"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridworksheet/filterstring/
---
## GridWorksheet.FilterString method

Définit le filtre pour la colonne. Notez que nous devons appeler AddAutoFilter avant d'appeler filterString. La chaîne de critères de filtre. Notez que nous utilisons la virgule-&gt;"," comme caractère de séparation, donc la valeur de cellule que vous souhaitez filtrer ne doit pas contenir de virgule. filterString(10,"123,456") signifie que la colonne 10 doit contenir 123 ou 456, filterString(10,"123") signifie que la colonne 10 doit contenir 123. L'index de colonne est séparé par des virgules, par ex. 123,456,789 ou abc

```csharp
public void FilterString(int column, string criteria)
```

### Voir aussi

* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


