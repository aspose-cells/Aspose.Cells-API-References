---
title: "TableStyleElement.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableStyleElement. Ottiene il tipo dell'elemento"
type: docs
url: /it/net/aspose.cells.tables/tablestyleelement/type/
---
## TableStyleElement.Type property

Ottiene il tipo dell'elemento.

```csharp
public TableStyleElementType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crea una tabella
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Ottieni lo stile della tabella (usando il nome dello stile invece di crearne uno nuovo)
            string styleName = table.TableStyleName;
            TableStyle style = workbook.Worksheets.TableStyles[styleName];

            // Accedi agli elementi di stile della tabella
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.HeaderRow];

            // Visualizza il tipo corrente dell'elemento
            Console.WriteLine("Current Type value: " + element.Type);

            // Nota: la proprietà Type è di sola lettura, quindi non possiamo impostarla
            // element.Type = TableStyleElementType.TotalRow; // Questo causerebbe un errore di compilazione

            // Dimostra come i diversi tipi di elemento influenzano la tabella
            Console.WriteLine("\nAvailable table style elements:");
            foreach (TableStyleElementType type in Enum.GetValues(typeof(TableStyleElementType)))
            {
                try
                {
                    TableStyleElement testElement = style.TableStyleElements[type];
                    Console.WriteLine($"Element type {type} exists in this style");
                }
                catch
                {
                    Console.WriteLine($"Element type {type} not available in this style");
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("TableStyleElementTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


