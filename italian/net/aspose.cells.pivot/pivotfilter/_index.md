---
title: "Classe PivotFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotFilter. Rappresenta un PivotFilter nella collezione PivotFilter"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/
---
## PivotFilter class

Rappresenta un PivotFilter nella collezione PivotFilter.

```csharp
public class PivotFilter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells.pivot/pivotfilter/autofilter/) { get; } | (**Obsolete.**) Ottiene l'autofiltro del filtro pivot. |
| [EvaluationOrder](../../aspose.cells.pivot/pivotfilter/evaluationorder/) { get; set; } | Ottiene l'ordine di valutazione del filtro pivot. |
| [FieldIndex](../../aspose.cells.pivot/pivotfilter/fieldindex/) { get; } | Ottiene l'indice del campo sorgente a cui è applicato questo filtro pivot. |
| [FilterCategory](../../aspose.cells.pivot/pivotfilter/filtercategory/) { get; } | Ottiene la categoria di questo filtro. |
| [FilterType](../../aspose.cells.pivot/pivotfilter/filtertype/) { get; } | Ottiene il tipo di filtro del filtro pivot. |
| [MeasureCubeFieldIndex](../../aspose.cells.pivot/pivotfilter/measurecubefieldindex/) { get; } | Specifica l'indice del campo cubo di misura. Questa proprietà è usata solo dai filtri nelle pivot OLAP e specifica su quale misura deve essere applicato un filtro di valore. |
| [MeasureFldIndex](../../aspose.cells.pivot/pivotfilter/measurefldindex/) { get; set; } | (**Obsolete.**) Ottiene l'indice del campo misura del filtro pivot. |
| [MemberPropertyFieldIndex](../../aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/) { get; set; } | Ottiene l'indice del campo proprietà membro del filtro pivot. |
| [Name](../../aspose.cells.pivot/pivotfilter/name/) { get; set; } | Ottiene il nome del filtro pivot. |
| [UseWholeDay](../../aspose.cells.pivot/pivotfilter/usewholeday/) { get; set; } | Indica se utilizzare giorni interi nei criteri di filtraggio della data. |
| [Value1](../../aspose.cells.pivot/pivotfilter/value1/) { get; set; } | Ottiene il valore stringa1 dell'etichetta del filtro pivot. |
| [Value2](../../aspose.cells.pivot/pivotfilter/value2/) { get; set; } | Ottiene il valore stringa2 dell'etichetta del filtro pivot. |
| [ValueFieldIndex](../../aspose.cells.pivot/pivotfilter/valuefieldindex/) { get; set; } | Restituisce l'indice del campo valore nella regione dei valori. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetDateTimeValues](../../aspose.cells.pivot/pivotfilter/getdatetimevalues/)() | Restituisce i valori del filtro numerico. |
| [GetLabels](../../aspose.cells.pivot/pivotfilter/getlabels/)() | Restituisce le etichette del filtro didascalia. |
| [GetNumberValues](../../aspose.cells.pivot/pivotfilter/getnumbervalues/)() | Restituisce i valori del filtro numerico. |
| [GetTop10Value](../../aspose.cells.pivot/pivotfilter/gettop10value/)() | Restituisce l'impostazione dei primi 10 del filtro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterDemo
    {
        public static void PivotFilterExample()
        {
            // Crea un nuovo workbook
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola il foglio di lavoro con dati di esempio
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Aggiungi una tabella pivot al foglio di lavoro
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Imposta lo stile della tabella pivot
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Aggiungi un filtro pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Imposta proprietà aggiuntive per il filtro pivot
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Aggiorna e calcola i dati della tabella pivot
            pivot.RefreshData();
            pivot.CalculateData();

            // Salva la cartella di lavoro
            book.Save("PivotFilterExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


