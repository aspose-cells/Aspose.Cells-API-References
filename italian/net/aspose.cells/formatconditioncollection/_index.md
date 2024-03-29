---
title: FormatConditionCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta la formattazione condizionale. FormatConditions può contenere fino a tre formati condizionali.
type: docs
weight: 3570
url: /it/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Rappresenta la formattazione condizionale. FormatConditions può contenere fino a tre formati condizionali.

```csharp
public class FormatConditionCollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count) { get; } | Ottiene il conteggio delle condizioni. |
| [Item](../../aspose.cells/formatconditioncollection/item) { get; } | Ottiene la condizione di formattazione per indice. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount) { get; } | Ottiene il conteggio degli intervalli formattati condizionalmente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add)(CellArea, FormatConditionType, OperatorType, string, string) | Aggiunge una condizione di formattazione e la cella effettuata ha suonato a FormatConditions FormatConditions può contenere fino a tre formati condizionali. Nelle formule di formattazione condizionale non sono consentiti riferimenti ad altri fogli. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea)(CellArea) | Aggiunge un intervallo di celle formattato condizionale. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition#addcondition)(FormatConditionType) | Aggiungi una condizione di formato. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition#addcondition_1)(FormatConditionType, OperatorType, string, string) | Aggiunge una condizione di formattazione. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea)(int) | Ottiene l'intervallo di celle formattato condizionale per indice. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea#removearea_1)(int) | Rimuove l'intervallo di celle formattato condizionale in base all'indice. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea#removearea)(int, int, int, int) | Rimuovi la formattazione condizionale nell'intervallo. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition)(int) | Rimuove la condizione di formattazione per indice. |

### Esempi

```csharp

[C#]

//Crea una nuova cartella di lavoro.
Workbook workbook = new Workbook();

//Ottieni il primo foglio di lavoro.
Worksheet sheet = workbook.Worksheets[0];

//Aggiunge una formattazione condizionale vuota
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
//Imposta l'intervallo di formato condizionale.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
//Aggiunge la condizione.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
//Aggiunge la condizione.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
//Imposta il colore di sfondo.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
//Salvataggio del file Excel
workbook.Save("output.xls");   

[Visual Basic]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
' Aggiunge una formattazione condizionale vuota
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
'Imposta l'intervallo di formato condizionale.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
'Aggiunge condizione.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
'Aggiunge condizione.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
'Imposta il colore di sfondo.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
'Salvataggio del file Excel
workbook.Save("output.xls")
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
