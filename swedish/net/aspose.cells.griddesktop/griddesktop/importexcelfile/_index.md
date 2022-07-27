---
title: ImportExcelFile
second_title: Aspose.Cells för .NET API-referens
description: Importerar från en Excel-filström inklusive diskfilström eller minnesström.
type: docs
weight: 730
url: /sv/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importerar från en Excel-filström, inklusive diskfilström eller minnesström.

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

* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importerar från en Excel-filström, inklusive diskfilström eller minnesström.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | strömobjekt. |
| runFormulas | Boolean | om det är sant kommer den här metoden att anropa metoden RunAllFormulas. |

### Se även

* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importerar från en excel-fil.

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

* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importerar från en excel-fil.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | excel filnamn. |
| runFormulas | Boolean | om det är sant kommer den här metoden att anropa metoden RunAllFormulas. |

### Se även

* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importerar från en excel-fil.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | Stream | ström av excel-fil. |
| passwordtoOpen | String | det öppna lösenordet för filen som är krypterad. |
| passwordtoOpen | String | ändringslösenordet för filen som är skyddad. |
| openasReadOnly | Boolean | om filen ska öppnas som skrivskyddad . |
| runFormulas | Boolean | om det är sant kommer den här metoden att anropa metoden RunAllFormulas. |

### Se även

* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importerar från en excel-fil.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | excel filnamn. |
| passwordtoOpen | String | det öppna lösenordet för filen som är krypterad. |
| passwordtoOpen | String | ändringslösenordet för filen som är skyddad. |
| openasReadOnly | Boolean | om filen ska öppnas som skrivskyddad . |
| runFormulas | Boolean | om det är sant kommer den här metoden att anropa metoden RunAllFormulas. |

### Se även

* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importerar ett kalkylblad från en excel-fil.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | excel filnamn. |
| sheetIndex | Int32 | index för ark som ska importeras. |

### Se även

* class [GridDesktop](../../griddesktop)
* namnutrymme [Aspose.Cells.GridDesktop](../../griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
