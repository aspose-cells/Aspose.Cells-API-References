---
title: "TableStyleElement.Size"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleElement‑Eigenschaft. Anzahl der Zeilen oder Spalten in einem einzelnen Streifenband. Gilt nur, wenn der Typ firstRowStripe, secondRowStripe, firstColumnStripe oder secondColumnStripe ist."
type: docs
url: /de/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

Anzahl der Zeilen oder Spalten in einem einzelnen Streifenband. Gilt nur, wenn der Typ firstRowStripe, secondRowStripe, firstColumnStripe oder secondColumnStripe ist.

```csharp
public int Size { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Eine Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Erstellen Sie einen Tabellenstil mithilfe der Stilsammlung des Arbeitsbuchs
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // Fügen Sie Streifenelemente hinzu, um die Size‑Eigenschaft zu demonstrieren
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // Greifen Sie auf die Streifenelemente zu
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // Aktuelle Size‑Werte anzeigen
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // Die Streifengrößen ändern
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // Geänderte Werte anzeigen
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


