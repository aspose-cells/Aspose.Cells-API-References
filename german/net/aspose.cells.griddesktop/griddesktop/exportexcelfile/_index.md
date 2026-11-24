---
title: "GridDesktop.ExportExcelFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridDesktop Methode. Exportiert in einen Excel-Dateistream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream"
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/exportexcelfile/
---
## ExportExcelFile(Stream) {#exportexcelfile}

Exportiert in einen Excel-Dateistream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream.

```csharp
public void ExportExcelFile(Stream stream)
```

### Beispiele

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

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}

Exportiert in einen Excel-Dateistream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream.

```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Stream, in dem die Kalkulationstabelle gespeichert wird. |
| fileFormatType | FileFormatType | Excel-Dateiformattyp. |

### Siehe auch

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string) {#exportexcelfile_2}

Exportiert in eine Excel-Datei.

```csharp
public void ExportExcelFile(string fileName)
```

### Beispiele

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

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}

Exportiert in eine Excel-Datei.

```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Der Name der erstellten Datei. |
| fileFormatType | FileFormatType | Excel-Dateiformattyp. |

### Siehe auch

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


