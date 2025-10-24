##GridDesktop.ImportExcelFile
GridDesktop method. Imports from an excel file stream including disk file stream or memory stream
## ImportExcelFile(Stream) {#importexcelfile}
Imports from an excel file stream, including disk file stream or memory stream.
```csharp
public void ImportExcelFile(Stream stream)
```
### Examples
```csharp
[C#]
private void button1_Click(object sender, System.EventArgs e)
{
FileStream fs = new FileStream("d:\\bookx.xls", FileMode.Open);
try
{
gridDesktop1.ImportExcelFile(fs);
}
catch(Exception ex)
{
}
finally
{
fs.Close();
}
}
[Visual Basic]
Private Sub menuItem1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles menuItem6.Click
Dim fs As FileStream =  New FileStream("d:\bookx.xls",FileMode.Open)
Try
gridDesktop1.ImportExcelFile(fs)
Catch ex As Exception
Throw ex
Finally
fs.Close()
End Try
End Sub
```
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ImportExcelFile(Stream, bool) {#importexcelfile_1}
Imports from an excel file stream, including disk file stream or memory stream.
```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | stream object. |
| runFormulas | Boolean | if true, this method will invoke RunAllFormulas method. |
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ImportExcelFile(string) {#importexcelfile_3}
Imports from an excel file.
```csharp
public void ImportExcelFile(string fileName)
```
### Examples
```csharp
[C#]
private void button1_Click(object sender, System.EventArgs e)
{
gridDesktop1.ImportExcelFile("FinancialPlan.xls");
}
[Visual Basic]
Private Sub menuItem1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles menuItem6.Click
gridDesktop1.ImportExcelFile("FinancialPlan.xls")
End Sub
```
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ImportExcelFile(string, bool) {#importexcelfile_4}
Imports from an excel file.
```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | excel file name. |
| runFormulas | Boolean | if true, this method will invoke RunAllFormulas method. |
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}
Imports from an excel file.
```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify,
bool openasReadOnly, bool runFormulas)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | stream of excel file . |
| passwordtoOpen | String | the open password for the file which is encrypted . |
| passwordtoModify | String | the modify password for the file which is protected . |
| openasReadOnly | Boolean | whether to open the file as ReadOnly . |
| runFormulas | Boolean | if true, this method will invoke RunAllFormulas method. |
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}
Imports from an excel file.
```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify,
bool openasReadOnly, bool runFormulas)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | excel file name. |
| passwordtoOpen | String | the open password for the file which is encrypted . |
| passwordtoModify | String | the modify password for the file which is protected . |
| openasReadOnly | Boolean | whether to open the file as ReadOnly . |
| runFormulas | Boolean | if true, this method will invoke RunAllFormulas method. |
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ImportExcelFile(string, int) {#importexcelfile_5}
Imports a worksheet from an excel file.
```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | excel file name. |
| sheetIndex | Int32 | index of sheet to be imported. |
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
