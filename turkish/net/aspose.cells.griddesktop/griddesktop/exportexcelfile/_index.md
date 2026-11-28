---
title: "GridDesktop.ExportExcelFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop yöntemi. Disk IO akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışına dışa aktarır"
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/exportexcelfile/
---
## ExportExcelFile(Stream) {#exportexcelfile}

Disk IO akışı veya bellek akışı dahil olmak üzere bir Excel dosya akışına dışa aktarır.

```csharp
public void ExportExcelFile(Stream stream)
```

### Örnekler

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

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}

Disk IO akışı veya bellek akışı dahil olmak üzere bir Excel dosya akışına dışa aktarır.

```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Elektronik tabloyu kaydetmek için akış. |
| fileFormatType | FileFormatType | Excel dosya formatı türü. |

### Ayrıca Bakınız

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string) {#exportexcelfile_2}

Bir Excel dosyasına dışa aktarır.

```csharp
public void ExportExcelFile(string fileName)
```

### Örnekler

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

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}

Bir Excel dosyasına aktarır.

```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | Oluşturulan dosyanın adı. |
| fileFormatType | FileFormatType | Excel dosya formatı türü. |

### Ayrıca Bakınız

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


