---
title: "CellsAI.BuildSpreadsheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsAI. Construir archivo de hoja de cálculo con la solicitud del usuario"
type: docs
url: /es/net/aspose.cells.ai/cellsai/buildspreadsheet/
---
## CellsAI.BuildSpreadsheet method

Crear archivo de hoja de cálculo con la solicitud del usuario

```csharp
public Task BuildSpreadsheet(string userRequest, string? inputFile, string outputFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| userRequest | String | la descripción de la solicitud para generar el archivo de hoja de cálculo |
| inputFile | String | la ruta completa del archivo de entrada, es opcional, si se desea modificar el archivo basado en este archivo, podemos establecerlo |
| outputFile | String | la ruta completa del archivo de salida |

### Ejemplos

Los siguientes ejemplos muestran cómo crear una hoja de cálculo bajo demanda

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

### Ver también

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


