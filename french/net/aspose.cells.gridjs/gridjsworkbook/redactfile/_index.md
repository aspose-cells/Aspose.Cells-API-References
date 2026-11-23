---
title: "GridJsWorkbook.RedactFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridJsWorkbook method. Effectue la rédaction d'un fichier Excel basé sur un tableau d'opérations JSON."
type: docs
url: /fr/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Effectue une rédaction sur un fichier Excel basée sur un tableau d'opérations JSON.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| excelFilePath | String | Le chemin du fichier Excel à rédiger. |
| uid | String | L'identifiant unique du classeur. Si null ou vide, un nouvel uid sera généré à partir du chemin du fichier. |
| arrayOfRedactionOpr | String[] | Un tableau de chaînes JSON représentant les opérations de rédaction à appliquer. |

### Exceptions

| exception | condition |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Lancé lorsqu'une CellsException se produit pendant l'opération de rédaction. |
| Exception | Lancé lorsqu'une exception générale se produit pendant l'opération de rédaction. |

### Voir aussi

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


