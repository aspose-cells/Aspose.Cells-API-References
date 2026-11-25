---
title: "TableStyleElementCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableStyleElementCollection. Ottiene un elemento dello stile della tabella per indice"
type: docs
url: /it/net/aspose.cells.tables/tablestyleelementcollection/item/
---
## TableStyleElementCollection indexer (1 of 2)

Ottiene un elemento dello stile della tabella per indice.

```csharp
public TableStyleElement this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

Restituisce l'oggetto [`TableStyleElement`](../../tablestyleelement/)

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Pattern = BackgroundType.Solid;
            firstColStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[elementIndex];
            element.SetElementStyle(firstColStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data");

            int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 1, 0, true);
            ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
            table.ShowTableStyleFirstColumn = true;
            table.TableStyleName = styleName;

            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleElement](../../tablestyleelement/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## TableStyleElementCollection indexer (2 of 2)

Ottiene l'elemento dello stile della tabella per tipo di elemento.

```csharp
public TableStyleElement this[TableStyleElementType type] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| type | Il tipo di elemento. |

### Valore di ritorno

Restituisce l'oggetto [`TableStyleElement`](../../tablestyleelement/)

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea uno stile di tabella personalizzato
            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Accedi a TableStyleElementCollection
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Aggiungi un elemento di stile della tabella
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);

            try
            {
                // Accedi alla proprietà Item usando l'indicizzatore (che utilizza internamente la proprietà Item)
                TableStyleElement element = elements[elementIndex];

                // Visualizza le informazioni sull'elemento
                Console.WriteLine("Table Style Element Type: " + element.Type);
                Console.WriteLine("Element has been successfully accessed via Item property");

                // Salva la cartella di lavoro
                workbook.Save("TableStyleElementItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [TableStyleElement](../../tablestyleelement/)
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


