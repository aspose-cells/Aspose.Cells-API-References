---
title: "Klass PivotItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotItem klass. Representerar ett objekt i en PivotField-rapport"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

Representerar ett item i en PivotField-rapport.

```csharp
public class PivotItem
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsolete.**) Hämtar indexet för pivotelementet i cache-fältet. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Anger om detta pivotelement är ett beräknat formelobjekt. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Hämtar och anger om detaljen för detta pivotelement är dold. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsolete.**) Anger om detta pivotelement är ett beräknat formelobjekt. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Hämtar och anger om pivotobjektet är dolt. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsolete.**) Hämtar och anger om pivotelementet döljer detaljen. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Anger om objektet har tagits bort från datakällan. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Hämtar namnet på pivotobjektet. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Anger indexet för detta objekt i alla PivotItems i fältet. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Föråldrad.**) Anger positionsindexet i PivotItems under samma föräldranod. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Hämtar värdet på pivotobjektet |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Hämtar datum/tidsvärdet för pivotobjektet. Om värdet är null, returneras DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Hämtar dubbelvärdet för pivotobjektet. Om värdet är null eller inte ett tal, returneras 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Hämtar formeln för detta beräknade objekt. Fungerar endast när detta objekt är ett beräknat objekt. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Hämtar strängvärdet för pivotobjektet. Om värdet är null, returneras "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | Flyttar objektet upp eller ner i pivåtfältet |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Föråldrad.**) Flyttar objektet upp eller ner |

## Fält

| Namn | Beskrivning |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | Välj-alla sentinel-index för sidobjekt (0x7FFD, inte ett giltigt index) |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Få åtkomst till pivåobjekten
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Skriv ut namnet på pivåobjektet
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Ställ in egenskaper
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Skriv ut värdet på pivåobjektet
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Använd metoder
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Spara arbetsboken
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


