---
title: ExportExcelFile
second_title: Aspose.Cells for .NET API 参考
description: 导出到 Excel 文件
type: docs
weight: 690
url: /zh/net/aspose.cells.griddesktop/griddesktop/exportexcelfile/
---
## ExportExcelFile(string) {#exportexcelfile_2}

导出到 Excel 文件。

```csharp
public void ExportExcelFile(string fileName)
```

### 例子

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

### 也可以看看

* class [GridDesktop](../../griddesktop)
* 命名空间 [Aspose.Cells.GridDesktop](../../griddesktop)
* 部件 [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}

导出到 Excel 文件。

```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 创建文件的名称。 |
| fileFormatType | FileFormatType | Excel 文件格式类型。 |

### 也可以看看

* enum [FileFormatType](../../fileformattype)
* class [GridDesktop](../../griddesktop)
* 命名空间 [Aspose.Cells.GridDesktop](../../griddesktop)
* 部件 [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream) {#exportexcelfile}

导出为excel文件流，包括磁盘IO流或内存流。

```csharp
public void ExportExcelFile(Stream stream)
```

### 例子

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

### 也可以看看

* class [GridDesktop](../../griddesktop)
* 命名空间 [Aspose.Cells.GridDesktop](../../griddesktop)
* 部件 [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}

导出为excel文件流，包括磁盘IO流或内存流。

```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 流式传输电子表格的保存位置。 |
| fileFormatType | FileFormatType | Excel 文件格式类型。 |

### 也可以看看

* enum [FileFormatType](../../fileformattype)
* class [GridDesktop](../../griddesktop)
* 命名空间 [Aspose.Cells.GridDesktop](../../griddesktop)
* 部件 [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
