---
title: "Cells.Find"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Trova la cella contenente l'oggetto di input"
type: docs
url: /it/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Trova la cella contenente l'oggetto di input.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cosa | Object | L'oggetto da cercare. Il tipo dovrebbe essere int,double,DateTime,string,bool. |
| previousCell | Cella | Cella precedente con lo stesso oggetto. Questo parametro può essere impostato a null se la ricerca inizia dall'inizio. |

### Valore di ritorno

Oggetto Cell.

### Osservazioni

Restituisce null (Nothing) se non viene trovata alcuna cella.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Trova la cella contenente "Orange"
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // Crea e applica uno stile alla cella trovata
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // Salva la cartella di lavoro
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Trova la cella contenente l'oggetto di input.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cosa | Object | L'oggetto da cercare. Il tipo dovrebbe essere int,double,DateTime,string,bool. |
| previousCell | Cella | Cella precedente con lo stesso oggetto. Questo parametro può essere impostato a null se la ricerca inizia dall'inizio. |
| findOptions | FindOptions | Opzioni di ricerca |

### Valore di ritorno

Oggetto Cell.

### Osservazioni

Restituisce null (Nothing) se non viene trovata alcuna cella.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellFindOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // Crea opzioni di ricerca
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Trova la cella con valore "abc "
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


