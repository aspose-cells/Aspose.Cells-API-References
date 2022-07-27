---
title: ImportExcelFile
second_title: Aspose.Cells for .NET API Referansı
description: Disk dosya akışı veya bellek akışı dahil olmak üzere bir excel dosya akışından içe aktarır.
type: docs
weight: 730
url: /tr/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Disk dosya akışı veya bellek akışı dahil olmak üzere bir excel dosya akışından içe aktarır.

```csharp
public void ImportExcelFile(Stream stream)
```

### Örnekler

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

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Disk dosya akışı veya bellek akışı dahil olmak üzere bir excel dosya akışından içe aktarır.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | akış nesnesi. |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Bir excel dosyasından içe aktarır.

```csharp
public void ImportExcelFile(string fileName)
```

### Örnekler

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

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Bir excel dosyasından içe aktarır.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | excel dosya adı |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Bir excel dosyasından içe aktarır.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | excel dosyası akışı. |
| passwordtoOpen | String | şifrelenen dosyanın açık parolası. |
| passwordtoOpen | String | korunan dosyanın parolasını değiştirin. |
| openasReadOnly | Boolean | dosyanın ReadOnly olarak açılıp açılmayacağı. |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Bir excel dosyasından içe aktarır.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | excel dosya adı |
| passwordtoOpen | String | şifrelenen dosyanın açık parolası. |
| passwordtoOpen | String | korunan dosyanın parolasını değiştirin. |
| openasReadOnly | Boolean | dosyanın ReadOnly olarak açılıp açılmayacağı. |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Excel dosyasından bir çalışma sayfasını içe aktarır.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | excel dosya adı |
| sheetIndex | Int32 | içe aktarılacak sayfanın dizini. |

### Ayrıca bakınız

* class [GridDesktop](../../griddesktop)
* ad alanı [Aspose.Cells.GridDesktop](../../griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
