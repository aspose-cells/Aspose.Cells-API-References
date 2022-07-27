---
title: ImportExcelFile
second_title: Aspose.Cells für .NET-API-Referenz
description: Importiert aus einem Excel-Dateistream einschließlich Disk-Dateistream oder Speicherstream.
type: docs
weight: 730
url: /de/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importiert aus einem Excel-Dateistream, einschließlich Disk-Dateistream oder Speicherstream.

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

* class [GridDesktop](../../griddesktop)
* namensraum [Aspose.Cells.GridDesktop](../../griddesktop)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importiert aus einem Excel-Dateistream, einschließlich Disk-Dateistream oder Speicherstream.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Stream-Objekt. |
| runFormulas | Boolean | wenn wahr, ruft diese Methode die RunAllFormulas-Methode auf. |

### Siehe auch

* class [GridDesktop](../../griddesktop)
* namensraum [Aspose.Cells.GridDesktop](../../griddesktop)
* Montage [Aspose.Cells.GridDesktop](../../../)

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

* class [GridDesktop](../../griddesktop)
* namensraum [Aspose.Cells.GridDesktop](../../griddesktop)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importiert aus einer Excel-Datei.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Excel-Dateiname. |
| runFormulas | Boolean | wenn wahr, ruft diese Methode die RunAllFormulas-Methode auf. |

### Siehe auch

* class [GridDesktop](../../griddesktop)
* namensraum [Aspose.Cells.GridDesktop](../../griddesktop)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importiert aus einer Excel-Datei.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Stream der Excel-Datei . |
| passwordtoOpen | String | das Öffnungskennwort für die verschlüsselte Datei . |
| passwordtoOpen | String | das Änderungskennwort für die geschützte Datei . |
| openasReadOnly | Boolean | ob die Datei als ReadOnly geöffnet werden soll. |
| runFormulas | Boolean | wenn wahr, ruft diese Methode die RunAllFormulas-Methode auf. |

### Siehe auch

* class [GridDesktop](../../griddesktop)
* namensraum [Aspose.Cells.GridDesktop](../../griddesktop)
* Montage [Aspose.Cells.GridDesktop](../../../)

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
| passwordtoOpen | String | das Öffnungskennwort für die verschlüsselte Datei . |
| passwordtoOpen | String | das Änderungskennwort für die geschützte Datei . |
| openasReadOnly | Boolean | ob die Datei als ReadOnly geöffnet werden soll. |
| runFormulas | Boolean | wenn wahr, ruft diese Methode die RunAllFormulas-Methode auf. |

### Siehe auch

* class [GridDesktop](../../griddesktop)
* namensraum [Aspose.Cells.GridDesktop](../../griddesktop)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importiert ein Arbeitsblatt aus einer Excel-Datei.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Excel-Dateiname. |
| sheetIndex | Int32 | Index des zu importierenden Blattes. |

### Siehe auch

* class [GridDesktop](../../griddesktop)
* namensraum [Aspose.Cells.GridDesktop](../../griddesktop)
* Montage [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
