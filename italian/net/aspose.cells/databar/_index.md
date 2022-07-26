---
title: DataBar
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Descrive la regola di formattazione condizionale DataBar. Questa regola di formattazione condizionale visualizza una barra dati graduata nellintervallo di celle.
type: docs
weight: 1240
url: /it/net/aspose.cells/databar/
---
## DataBar class

Descrive la regola di formattazione condizionale DataBar. Questa regola di formattazione condizionale visualizza una barra dati graduata nell'intervallo di celle.

```csharp
public class DataBar
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | Ottiene il colore dell'asse per le celle con formattazione condizionale come barre di dati. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | Ottiene o imposta la posizione dell'asse delle barre dei dati specificata da una regola di formattazione condizionale. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | Ottiene un oggetto che specifica il bordo di una barra dati. |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | Ottiene o imposta la modalità di riempimento di una barra dati con il colore. |
| [Color](../../aspose.cells/databar/color) { get; set; } | Ottieni o imposta il colore di questa DataBar. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | Ottiene o imposta la direzione in cui viene visualizzata la barra dati. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | Ottieni o imposta l'oggetto valore massimo di questo DataBar. Impossibile impostare null o CFValueObject con il tipo FormatConditionValueType.Min su di esso. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | Rappresenta la lunghezza massima della barra dei dati. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | Ottieni o imposta l'oggetto valore minimo di questo DataBar. Impossibile impostare null o CFValueObject con tipo FormatConditionValueType.Max su di esso. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | Rappresenta la lunghezza minima della barra dei dati. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | Ottiene l'oggetto NegativeBarFormat associato a una regola di formattazione condizionale della barra dati. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | Ottieni o imposta il flag che indica se mostrare i valori delle celle su cui è applicata questa barra dati. Il valore predefinito è true. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | Visualizza la barra dei dati nella cella nell'array di byte dell'immagine. |

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Aggiunge una formattazione condizionale vuota
int index = sheet.ConditionalFormattings.Add();

FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

//Imposta l'intervallo di formato condizionale.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

//Aggiunge la condizione.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

//Ottieni la barra dati
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

//Imposta le proprietà della barra dati
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;

dataBar.MinCfvo.Value = 30;

dataBar.ShowValue = false;

dataBar.BarBorder.Type = DataBarBorderType.Solid;

dataBar.BarBorder.Color = Color.Plum;

 dataBar.BarFillType = DataBarFillType.Solid;
  
 dataBar.AxisColor = Color.Red;
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.Color = Color.White;
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
 
//Inserisci i valori delle celle
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

//Salvataggio del file Excel
workbook.Save("book1.xlsx");

[VB.NET]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Aggiunge una formattazione condizionale vuota
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'Imposta l'intervallo di formato condizionale.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'Aggiunge condizione.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'Ottieni la barra dati
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'Imposta le proprietà della barra dati
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile

dataBar.MinCfvo.Value = 30

dataBar.ShowValue = False

dataBar.BarBorder.Type = DataBarBorderType.Solid

dataBar.BarBorder.Color = Color.Plum

 dataBar.BarFillType = DataBarFillType.Solid
  
 dataBar.AxisColor = Color.Red
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.Color = Color.White
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow

'Metti i valori delle celle
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'Salvataggio del file Excel
workbook.Save("book1.xlsx")

```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
