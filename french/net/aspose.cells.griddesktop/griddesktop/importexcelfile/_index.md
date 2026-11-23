---
title: "GridDesktop.ImportExcelFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridDesktop method. Importe depuis un flux de fichier Excel, y compris le flux de fichier disque ou le flux mémoire"
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importe depuis un flux de fichier Excel, y compris un flux de fichier disque ou un flux mémoire.

```csharp
public void ImportExcelFile(Stream stream)
```

### Exemples

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

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importe depuis un flux de fichier Excel, y compris un flux de fichier disque ou un flux mémoire.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | objet de flux. |
| runFormulas | Boolean | si vrai, cette méthode appellera la méthode RunAllFormulas. |

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importe depuis un fichier Excel.

```csharp
public void ImportExcelFile(string fileName)
```

### Exemples

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

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importe depuis un fichier Excel.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | nom du fichier Excel. |
| runFormulas | Boolean | si vrai, cette méthode appellera la méthode RunAllFormulas. |

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importe depuis un fichier Excel.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | flux du fichier Excel. |
| passwordtoOpen | String | le mot de passe d'ouverture du fichier qui est chiffré. |
| passwordtoModify | String | le mot de passe de modification du fichier qui est protégé. |
| openasReadOnly | Boolean | indique si le fichier doit être ouvert en lecture seule. |
| runFormulas | Boolean | si vrai, cette méthode appellera la méthode RunAllFormulas. |

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importe depuis un fichier Excel.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | nom du fichier Excel. |
| passwordtoOpen | String | le mot de passe d'ouverture du fichier qui est chiffré. |
| passwordtoModify | String | le mot de passe de modification du fichier qui est protégé. |
| openasReadOnly | Boolean | indique si le fichier doit être ouvert en lecture seule. |
| runFormulas | Boolean | si vrai, cette méthode appellera la méthode RunAllFormulas. |

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importe une feuille de calcul depuis un fichier Excel.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | nom du fichier Excel. |
| sheetIndex | Int32 | indice de la feuille à importer. |

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


