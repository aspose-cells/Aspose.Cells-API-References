---
title: "Worksheet.FilterString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Définit le filtre pour la colonne. Notez que nous devons appeler AddAutoFilter avant d’appeler filterString. La chaîne de critères du filtre. Notez que nous utilisons la virgule comme caractère de séparation, donc la valeur de cellule que vous souhaitez filtrer ne doit pas contenir de virgule. filterString10123456 signifie que la colonne 10 doit contenir 123 ou 456. filterString10123 signifie que la colonne 10 doit contenir 123, valeur séparée par des virgules, par ex. 123456789 ou abc"
type: docs
url: /fr/net/aspose.cells.griddesktop/worksheet/filterstring/
---
## Worksheet.FilterString method

Définit le filtre pour la colonne. Notez que nous devons appeler AddAutoFilter avant d'appeler filterString. Chaîne de critères du filtre. Notez que nous utilisons la virgule-&gt;\",\" comme caractère de séparation, donc la valeur de cellule que vous souhaitez filtrer ne doit pas contenir de virgule. filterString(10,\"123,456\") signifie que la colonne 10 doit contenir 123 ou 456, filterString(10,\"123\") signifie que la colonne 10 doit contenir la valeur 123 séparée par des virgules, par ex. 123,456,789 ou abc

```csharp
public void FilterString(int column, string criteria)
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


