##GridDesktop.ExportExcelFile
GridDesktop method. Exports to a excel file stream including disk IO stream or memory stream
## ExportExcelFile(Stream) {#exportexcelfile}
Exports to a excel file stream, including disk IO stream or memory stream.
```csharp
public void ExportExcelFile(Stream stream)
```
### Examples
```csharp
[C#]
private void button1_Click(object sender, System.EventArgs e)
{
FileStream fs = new FileStream("d:\\bookx.xls", FileMode.OpenOrCreate);
try
{
gridDesktop1.Worksheets.ExportExcelFile(fs);
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
Dim fs As FileStream =  New FileStream("d:\bookx.xls", FileMode.OpenOrCreate)
Try
gridDesktop1.Worksheets.ExportExcelFile(fs)
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
## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}
Exports to a excel file stream, including disk IO stream or memory stream.
```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | Stream where to save the spreadsheet. |
| fileFormatType | FileFormatType | Excel file format type. |
### See Also
* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ExportExcelFile(string) {#exportexcelfile_2}
Exports to an excel file.
```csharp
public void ExportExcelFile(string fileName)
```
### Examples
```csharp
[C#]
private void button1_Click(object sender, System.EventArgs e)
{
gridDesktop1.Worksheets.ExportExcelFile("savedemo.xls");
}
[Visual Basic]
Private Sub menuItem1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles menuItem7.Click
gridDesktop1.Worksheets.ExportExcelFile("savedemo.xls")
End Sub
```
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}
Exports to a excel file.
```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The name of created file. |
| fileFormatType | FileFormatType | Excel file format type. |
### See Also
* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
