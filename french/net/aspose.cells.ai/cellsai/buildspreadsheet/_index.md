---
title: "CellsAI.BuildSpreadsheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsAI. Construire le fichier de feuille de calcul avec la demande de l'utilisateur"
type: docs
url: /fr/net/aspose.cells.ai/cellsai/buildspreadsheet/
---
## CellsAI.BuildSpreadsheet method

Créer un fichier Spreadsheet avec la demande de l'utilisateur

```csharp
public Task BuildSpreadsheet(string userRequest, string? inputFile, string outputFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| userRequest | String | la description de la demande pour générer le fichier de feuille de calcul |
| inputFile | String | le chemin complet du fichier d'entrée, il est optionnel, si vous voulez modifier le fichier basé sur ce fichier, vous pouvez le définir |
| outputFile | String | le chemin complet du fichier de sortie |

### Exemples

Les exemples suivants montrent comment créer une feuille de calcul à la demande

```csharp
[C#]
Config.Model=Model.Gpt4OMini;
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String userRequest = @"Provide weekly daily three-meal recipes, including nutritional value, preparation methods, ingredients, and cost ,one day per row,and add total cost at last row.";
String outfile = "D:\\foodsweekly.xlsx";
await cellsAI.BuildSpreadsheet(userRequest, null, outfile);

String userRequest = @"Based on the sales history data from row 3 to row 10, predict the sales situation for the next year.add it in row 11.";
String outfile = "D:\\Sales Report Forcast.xlsx";
String inputfile = "D:\\Sales Report Year.xlsx";
await cellsAI.BuildSpreadsheet(userRequest, inputfile, outfile);

String userRequest = "Change the background colors of the rows where the top three highest year sales are located to red, yellow, and green, respectively.";
String outfile = "D:\\Sales Report Top3.xlsx";
String inputfile = "D:\\Sales Report Year.xlsx";
await cellsAI.BuildSpreadsheet(userRequest, inputfile, outfile);

String userRequest = "Add a new column named \"Ranking\" and fill in the content of this column based on the students' total scores ranking.";
String outfile = "D:\\student_score_with_rank.xlsx";
String inputfile = "D:\\student_score.xlsx";
await cellsAI.BuildSpreadsheet(userRequest, inputfile, outfile);

Config.Model=Model.QwenPlus;
Config.Locale = "zh";
String userRequest ="增加新的一列,列名称是\"排名\" 并根据学生的总分大小排名填入这一列的内容";
String outfile = "D:\\学生排行.xlsx";
String inputfile = "D:\\student_score_zh.xlsx";
await cellsAI.BuildSpreadsheet(userRequest, inputfile, outfile);


String userRequest = "总分成绩最好的学生所在的行背景色改为绿色，成绩最差的学生的背景色改为黄色，把分数不及格的单元格用红色标记出来";
String outfile = "D:\\学生排行信息.xlsx";
String inputfile = "D:\\student_score_zh.xlsx";
await cellsAI.BuildSpreadsheet(userRequest, inputfile, outfile);
```

### Voir aussi

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


