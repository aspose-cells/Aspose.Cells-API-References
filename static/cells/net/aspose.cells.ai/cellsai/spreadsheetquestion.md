##CellsAI.SpreadsheetQuestion
CellsAI method. Get answer of the question from the spreadsheetusing TextWriter to write the result
## SpreadsheetQuestion(string, string, TextWriter) {#spreadsheetquestion_1}
Get answer of the question from the spreadsheet,using TextWriter to write the result
```csharp
public Task SpreadsheetQuestion(string path, string question, TextWriter writer)
```
| Parameter | Type | Description |
| --- | --- | --- |
| path | String | the file path |
| question | String | the question |
| writer | TextWriter | the TextWriter to write the result |
### See Also
* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)
## SpreadsheetQuestion(string, string) {#spreadsheetquestion}
Get answer of the question from the spreadsheet
```csharp
public string SpreadsheetQuestion(string path, string question)
```
| Parameter | Type | Description |
| --- | --- | --- |
| path | String | the file path |
| question | String | the question |
### Return Value
AI query response
### Examples
```csharp
[C#]
CellsAI cellsAI = new CellsAI(AIRootUrl, AIKey);
String question = @"Which year had the highest total sales revenue?";
String path = "D:\\sales_report.xlsx";
String ret= cellsAI.SpreadsheetQuestion(path, question);
```
### See Also
* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [CellsAI](../../../)
