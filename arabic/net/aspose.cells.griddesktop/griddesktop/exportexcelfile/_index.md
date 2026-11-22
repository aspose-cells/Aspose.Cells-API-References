---
title: "GridDesktop.ExportExcelFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridDesktop. تصدر إلى تدفق ملف إكسل بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/exportexcelfile/
---
## ExportExcelFile(Stream) {#exportexcelfile}

يصدّر إلى تدفق ملف إكسل، بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة.

```csharp
public void ExportExcelFile(Stream stream)
```

### أمثلة

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

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}

يصدّر إلى تدفق ملف إكسل، بما في ذلك تدفق إدخال/إخراج القرص أو تدفق الذاكرة.

```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | التدفق حيث يتم حفظ جدول البيانات. |
| fileFormatType | FileFormatType | نوع تنسيق ملف إكسل. |

### انظر أيضًا

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string) {#exportexcelfile_2}

يصدّر إلى ملف إكسل.

```csharp
public void ExportExcelFile(string fileName)
```

### أمثلة

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

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}

يصدّر إلى ملف إكسل.

```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم الملف الذي تم إنشاؤه. |
| fileFormatType | FileFormatType | نوع تنسيق ملف إكسل. |

### انظر أيضًا

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


