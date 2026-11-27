---
title: "GridDesktop.ImportExcelFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridDesktop metod. Importerar från en Excel-filström inklusive filström från disk eller minnesström"
type: docs
url: /sv/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importerar från en Excel-filström, inklusive filström från disk eller minnesström.

```csharp
public void ImportExcelFile(Stream stream)
```

### Exempel

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

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importerar från en Excel-filström, inklusive filström från disk eller minnesström.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | strömobjekt. |
| runFormulas | Boolean | om sant, kommer denna metod att anropa RunAllFormulas-metoden. |

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importerar från en Excel-fil.

```csharp
public void ImportExcelFile(string fileName)
```

### Exempel

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

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importerar från en Excel-fil.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | excel-filnamn. |
| runFormulas | Boolean | om sant, kommer denna metod att anropa RunAllFormulas-metoden. |

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importerar från en Excel-fil.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | ström av excel-fil . |
| passwordtoOpen | String | det öppna lösenordet för den fil som är krypterad . |
| passwordtoModify | String | det modifieringslösenordet för den fil som är skyddad . |
| openasReadOnly | Boolean | om filen ska öppnas som ReadOnly . |
| runFormulas | Boolean | om sant, kommer denna metod att anropa RunAllFormulas-metoden. |

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importerar från en Excel-fil.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | excel-filnamn. |
| passwordtoOpen | String | det öppna lösenordet för den fil som är krypterad . |
| passwordtoModify | String | det modifieringslösenordet för den fil som är skyddad . |
| openasReadOnly | Boolean | om filen ska öppnas som ReadOnly . |
| runFormulas | Boolean | om sant, kommer denna metod att anropa RunAllFormulas-metoden. |

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importerar ett kalkylblad från en excel‑fil.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | excel-filnamn. |
| sheetIndex | Int32 | index för blad som ska importeras. |

### Se även

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


