---
title: "GridDesktop.ImportExcelFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridDesktop. Importa da un flusso di file Excel, inclusi flusso da file su disco o flusso di memoria"
type: docs
url: /it/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importa da un flusso di file Excel, includendo flusso da disco o flusso di memoria.

```csharp
public void ImportExcelFile(Stream stream)
```

### Esempi

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

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importa da un flusso di file Excel, includendo flusso da disco o flusso di memoria.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | oggetto stream. |
| runFormulas | Booleano | se vero, questo metodo invocherà il metodo RunAllFormulas. |

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importa da un file Excel.

```csharp
public void ImportExcelFile(string fileName)
```

### Esempi

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

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importa da un file Excel.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | nome del file excel. |
| runFormulas | Booleano | se vero, questo metodo invocherà il metodo RunAllFormulas. |

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importa da un file Excel.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | flusso del file excel. |
| passwordtoOpen | String | la password di apertura per il file che è crittografato. |
| passwordtoModify | String | la password di modifica per il file che è protetto. |
| openasReadOnly | Booleano | se aprire il file in sola lettura. |
| runFormulas | Booleano | se vero, questo metodo invocherà il metodo RunAllFormulas. |

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importa da un file Excel.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | nome del file excel. |
| passwordtoOpen | String | la password di apertura per il file che è crittografato. |
| passwordtoModify | String | la password di modifica per il file che è protetto. |
| openasReadOnly | Booleano | se aprire il file in sola lettura. |
| runFormulas | Booleano | se vero, questo metodo invocherà il metodo RunAllFormulas. |

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importa un foglio di lavoro da un file Excel.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | String | nome del file excel. |
| sheetIndex | Int32 | indice del foglio da importare. |

### Vedi anche

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


