---
title: "CellsAI.SpreadsheetQuestion"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsAI. Obtenir la réponse à la question depuis la feuille de calcul en utilisant TextWriter pour écrire le résultat"
type: docs
url: /fr/net/aspose.cells.ai/cellsai/spreadsheetquestion/
---
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}

Obtenir la réponse à la question depuis la feuille de calcul, en utilisant TextWriter pour écrire le résultat

```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | le chemin du fichier |
| question | String | la question |
| écrivain | TextWriter | le TextWriter pour écrire le résultat |

### Voir aussi

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)

---

## SpreadsheetQuestion(string, string) {#spreadsheetquestion}

Obtenir la réponse à la question depuis la feuille de calcul

```csharp
public string SpreadsheetQuestion(string path, string question)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | le chemin du fichier |
| question | String | la question |

### Valeur de retour

Réponse de la requête IA

### Exemples

```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```

### Voir aussi

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


