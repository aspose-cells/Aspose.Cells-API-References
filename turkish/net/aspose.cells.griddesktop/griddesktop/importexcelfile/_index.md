---
title: "GridDesktop.ImportExcelFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridDesktop method. Disk dosyası akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır"
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Disk dosya akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır.

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

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Disk dosya akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | akış nesnesi. |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Bir Excel dosyasından içe aktarır.

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

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Bir Excel dosyasından içe aktarır.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | excel dosya adı. |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Bir Excel dosyasından içe aktarır.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | excel dosyasının akışı. |
| passwordtoOpen | String | şifrelenmiş dosya için açma şifresi. |
| passwordtoModify | String | korumalı dosya için değiştirme şifresi. |
| openasReadOnly | Boolean | dosyayı yalnızca okunur olarak açıp açmayacağını belirler. |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Bir Excel dosyasından içe aktarır.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | excel dosya adı. |
| passwordtoOpen | String | şifrelenmiş dosya için açma şifresi. |
| passwordtoModify | String | korumalı dosya için değiştirme şifresi. |
| openasReadOnly | Boolean | dosyayı yalnızca okunur olarak açıp açmayacağını belirler. |
| runFormulas | Boolean | true ise, bu yöntem RunAllFormulas yöntemini çağırır. |

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Bir Excel dosyasından çalışma sayfası içe aktarır.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | excel dosya adı. |
| sheetIndex | Int32 | içe aktarılacak sayfanın indeksi. |

### Ayrıca Bakınız

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


