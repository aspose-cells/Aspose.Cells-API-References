---
title: ImportExcelFile
second_title: Référence de l'API Aspose.Cells pour .NET
description: Importations à partir dun flux de fichiers Excel y compris le flux de fichiers de disque ou le flux de mémoire.
type: docs
weight: 730
url: /fr/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importations à partir d'un flux de fichiers Excel, y compris le flux de fichiers de disque ou le flux de mémoire.

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

### Voir également

* class [GridDesktop](../../griddesktop)
* espace de noms [Aspose.Cells.GridDesktop](../../griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importations à partir d'un flux de fichiers Excel, y compris le flux de fichiers de disque ou le flux de mémoire.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | objet flux. |
| runFormulas | Boolean | si vrai, cette méthode invoquera la méthode RunAllFormulas. |

### Voir également

* class [GridDesktop](../../griddesktop)
* espace de noms [Aspose.Cells.GridDesktop](../../griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importe à partir d'un fichier Excel.

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

### Voir également

* class [GridDesktop](../../griddesktop)
* espace de noms [Aspose.Cells.GridDesktop](../../griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importe à partir d'un fichier Excel.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | nom du fichier excel. |
| runFormulas | Boolean | si vrai, cette méthode invoquera la méthode RunAllFormulas. |

### Voir également

* class [GridDesktop](../../griddesktop)
* espace de noms [Aspose.Cells.GridDesktop](../../griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importe à partir d'un fichier Excel.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | flux de fichier excel. |
| passwordtoOpen | String | le mot de passe d'ouverture du fichier qui est crypté. |
| passwordtoOpen | String | le mot de passe de modification du fichier protégé . |
| openasReadOnly | Boolean | s'il faut ouvrir le fichier en tant que ReadOnly . |
| runFormulas | Boolean | si vrai, cette méthode invoquera la méthode RunAllFormulas. |

### Voir également

* class [GridDesktop](../../griddesktop)
* espace de noms [Aspose.Cells.GridDesktop](../../griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importe à partir d'un fichier Excel.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | nom du fichier excel. |
| passwordtoOpen | String | le mot de passe d'ouverture du fichier qui est crypté. |
| passwordtoOpen | String | le mot de passe de modification du fichier protégé . |
| openasReadOnly | Boolean | s'il faut ouvrir le fichier en tant que ReadOnly . |
| runFormulas | Boolean | si vrai, cette méthode invoquera la méthode RunAllFormulas. |

### Voir également

* class [GridDesktop](../../griddesktop)
* espace de noms [Aspose.Cells.GridDesktop](../../griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importe une feuille de calcul à partir d'un fichier Excel.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | nom du fichier excel. |
| sheetIndex | Int32 | index de la feuille à importer. |

### Voir également

* class [GridDesktop](../../griddesktop)
* espace de noms [Aspose.Cells.GridDesktop](../../griddesktop)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
