---
title: "GridDesktop.ExportExcelFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop metod. Exporterar till en Excel-filström inklusive disk-IO-ström eller minnesström"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/exportexcelfile/
---
## ExportExcelFile(Stream) {#exportexcelfile}

Exporterar till en excel‑filström, inklusive disk‑IO‑ström eller minnesström.

```csharp
public void ExportExcelFile(Stream stream)
```

### Exempel

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

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}

Exporterar till en excel‑filström, inklusive disk‑IO‑ström eller minnesström.

```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Ström där kalkylbladet ska sparas. |
| fileFormatType | FileFormatType | Excel-filformatstyp. |

### Se även

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string) {#exportexcelfile_2}

Exporterar till en excel‑fil.

```csharp
public void ExportExcelFile(string fileName)
```

### Exempel

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

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}

Exporterar till en excel‑fil.

```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | Namnet på den skapade filen. |
| fileFormatType | FileFormatType | Excel-filformatstyp. |

### Se även

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


