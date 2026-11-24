---
title: "GridDesktop.ImportExcelFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridDesktop Methode. Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstrom."
type: docs
url: /de/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstream.

```csharp
public void ImportExcelFile(Stream stream)
```

### Beispiele

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

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstream.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Stream-Objekt. |
| runFormulas | Boolean | Wenn true, ruft diese Methode die Methode RunAllFormulas auf. |

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importiert aus einer Excel-Datei.

```csharp
public void ImportExcelFile(string fileName)
```

### Beispiele

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

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importiert aus einer Excel-Datei.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Excel-Dateiname. |
| runFormulas | Boolean | Wenn true, ruft diese Methode die Methode RunAllFormulas auf. |

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importiert aus einer Excel-Datei.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | Stream einer Excel-Datei. |
| passwordtoOpen | String | das Öffnungspasswort für die Datei, die verschlüsselt ist . |
| passwordtoModify | String | das Änderungskennwort für die Datei, die geschützt ist . |
| openasReadOnly | Boolean | ob die Datei als Nur-Lesen geöffnet werden soll . |
| runFormulas | Boolean | Wenn true, ruft diese Methode die Methode RunAllFormulas auf. |

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importiert aus einer Excel-Datei.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Excel-Dateiname. |
| passwordtoOpen | String | das Öffnungspasswort für die Datei, die verschlüsselt ist . |
| passwordtoModify | String | das Änderungskennwort für die Datei, die geschützt ist . |
| openasReadOnly | Boolean | ob die Datei als Nur-Lesen geöffnet werden soll . |
| runFormulas | Boolean | Wenn true, ruft diese Methode die Methode RunAllFormulas auf. |

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importiert ein Arbeitsblatt aus einer Excel-Datei.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Excel-Dateiname. |
| sheetIndex | Int32 | Index des zu importierenden Blatts. |

### Siehe auch

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


