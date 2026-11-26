---
title: "GridDesktop.ExportExcelFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridDesktop. Экспортирует в поток Excel-файла, включая поток ввода-вывода диска или поток памяти"
type: docs
url: /ru/net/aspose.cells.griddesktop/griddesktop/exportexcelfile/
---
## ExportExcelFile(Stream) {#exportexcelfile}

Экспортирует в поток Excel‑файла, включая поток ввода‑вывода диска или поток памяти.

```csharp
public void ExportExcelFile(Stream stream)
```

### Примеры

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

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}

Экспортирует в поток Excel‑файла, включая поток ввода‑вывода диска или поток памяти.

```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Поток, в который сохраняется таблица. |
| fileFormatType | FileFormatType | Тип формата Excel-файла. |

### См. также

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string) {#exportexcelfile_2}

Экспортирует в Excel‑файл.

```csharp
public void ExportExcelFile(string fileName)
```

### Примеры

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

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}

Экспортирует в файл Excel.

```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | Имя созданного файла. |
| fileFormatType | FileFormatType | Тип формата Excel-файла. |

### См. также

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


