---
title: "CellsAI.BuildSpreadsheet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellsAI 方法。根据用户请求构建电子表格文件"
type: docs
url: /zh/net/aspose.cells.ai/cellsai/buildspreadsheet/
---
## CellsAI.BuildSpreadsheet method

根据用户请求构建电子表格文件

```csharp
public Task BuildSpreadsheet(string userRequest, string? inputFile, string outputFile)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| userRequest | String | 用于生成电子表格文件的请求描述 |
| inputFile | String | 输入文件的完整路径，可选；如果想基于此文件进行修改，可以设置它 |
| outputFile | String | 输出文件的完整路径 |

### 示例

以下示例展示了如何按需构建电子表格

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

### 另请参见

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)


