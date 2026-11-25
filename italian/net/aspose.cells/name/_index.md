---
title: "Nome della classe"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Name class. Rappresenta un nome definito per un intervallo di celle"
type: docs
url: /it/net/aspose.cells/name/
---
## Name class

Rappresenta un nome definito per un intervallo di celle.

```csharp
public class Name
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | Ottiene e imposta il commento del nome. Si applica solo a Excel 2007 o versioni successive. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | Ottiene il testo completo del nome dell'oggetto con l'impostazione di ambito. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | Indica se questo nome è referenziato da altre formule. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | Indica se il nome è visibile. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | Ottiene o imposta un riferimento R1C1 del `Name`. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | Restituisce o imposta la formula a cui il nome è definito per riferirsi, iniziando con il segno di uguale. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | Indica a quale cartella di lavoro o foglio appartiene questo nome. 0 = Nome globale, altrimenti indice al foglio (basato su 1). |
| [Text](../../aspose.cells/name/text/) { get; set; } | Ottiene il testo del nome dell'oggetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | Ottiene l'intervallo se questo nome si riferisce a un intervallo. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | Ottiene l'intervallo se questo nome si riferisce a un intervallo |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | Ottiene l'intervallo se questo nome si riferisce a un intervallo. Se il riferimento di questo nome non è assoluto, l'intervallo può variare per celle diverse. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | Ottiene tutti gli intervalli referenziati da questo nome. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | Ottiene tutti gli intervalli referenziati da questo nome. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | Ottiene tutti i riferimenti referenziati da questo nome. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | Ottieni il riferimento di questo Name. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | Ottieni il riferimento di questo Name basato sulla cella specificata. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | Imposta il riferimento di questo Name. |
| override [ToString](../../aspose.cells/name/tostring/)() | Restituisce una stringa che rappresenta l'oggetto Range corrente. |

### Esempi

```csharp

[C#]

//Istanziare un oggetto Workbook
Workbook workbook = new Workbook();
//Accesso al primo foglio di lavoro nel file Excel
Worksheet worksheet = workbook.Worksheets[0];
//Creazione di un intervallo denominato
Range range = worksheet.Cells.CreateRange("B4", "G14");
//Impostazione del nome dell'intervallo denominato
range.Name = "TestRange";
//Salvataggio del file Excel modificato nel formato predefinito (cioè Excel 2000)
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Creating a named range
Dim range As Range = worksheet.Cells.CreateRange("B4", "G14")
'Setting the name of the named range
range.Name = "TestRange"
'Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save("output.xls")
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


