---
title: "GridDesktop.ExportExcelFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridDesktop. Exporte vers un flux de fichier Excel incluant un flux d'E/S disque ou un flux mémoire"
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/exportexcelfile/
---
## ExportExcelFile(Stream) {#exportexcelfile}

Exporte vers un flux de fichier Excel, incluant le flux d'E/S disque ou le flux mémoire.

```csharp
public void ExportExcelFile(Stream stream)
```

### Exemples

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

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(Stream, FileFormatType) {#exportexcelfile_1}

Exporte vers un flux de fichier Excel, incluant le flux d'E/S disque ou le flux mémoire.

```csharp
public void ExportExcelFile(Stream stream, FileFormatType fileFormatType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Flux où enregistrer la feuille de calcul. |
| fileFormatType | FileFormatType | Type de format de fichier Excel. |

### Voir aussi

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string) {#exportexcelfile_2}

Exporte vers un fichier Excel.

```csharp
public void ExportExcelFile(string fileName)
```

### Exemples

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

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ExportExcelFile(string, FileFormatType) {#exportexcelfile_3}

Exporte vers un fichier Excel.

```csharp
public void ExportExcelFile(string fileName, FileFormatType fileFormatType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom du fichier créé. |
| fileFormatType | FileFormatType | Type de format de fichier Excel. |

### Voir aussi

* enum [FileFormatType](../../fileformattype/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


