---
title: "Classe PivotItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotItem. Rappresenta un elemento in un report PivotField"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

Rappresenta un elemento in un report PivotField.

```csharp
public class PivotItem
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsoleto.**) Ottiene l'indice dell'elemento pivot nel campo cache. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Indica se questo elemento pivot è un elemento di formula calcolata. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Ottiene e imposta se il dettaglio di questo elemento pivot è nascosto. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsoleto.**) Indica se questo elemento pivot è un elemento di formula calcolata. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Ottiene e imposta se l'elemento pivot è nascosto. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsoleto.**) Ottiene e imposta se l'elemento pivot nasconde il dettaglio. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Indica se l'elemento è stato rimosso dalla fonte dati. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Ottiene il nome dell'elemento pivot. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Specificando l'indice di questo elemento in tutti i PivotItems del campo. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Obsoleto.**) Specificando l'indice di posizione nei PivotItems sotto lo stesso nodo genitore. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Ottiene il valore dell'elemento pivot |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Ottiene il valore data/ora dell'elemento pivot. Se il valore è null, restituisce DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Restituisce il valore double dell'elemento pivot. Se il valore è nullo o non è un numero, restituisce 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Ottiene la formula di questo elemento calcolato. Funziona solo quando questo elemento è calcolato. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Restituisce il valore stringa dell'elemento pivot. Se il valore è nullo, restituisce "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | Sposta l'elemento su o giù nel campo pivot |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Obsoleto.**) Sposta l'elemento su o giù |

## Campi

| Nome | Descrizione |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | Indice sentinella di selezione totale degli elementi di pagina (0x7FFD, indice non valido) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemDemo
    {
        public static void PivotItemExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi una tabella pivot al foglio di lavoro
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accedi agli elementi pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Stampa il nome dell'elemento pivot
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Imposta le proprietà
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Stampa il valore dell'elemento pivot
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Usa i metodi
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


