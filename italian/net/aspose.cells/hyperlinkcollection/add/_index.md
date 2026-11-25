---
title: "HyperlinkCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo HyperlinkCollection. Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle."
type: docs
url: /it/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Prima riga dell'intervallo di collegamenti ipertestuali. |
| firstColumn | Int32 | Prima colonna dell'intervallo di collegamenti ipertestuali. |
| totalRows | Int32 | Numero di righe in questo intervallo di collegamenti ipertestuali. |
| totalColumns | Int32 | Numero di colonne di questo intervallo di collegamenti ipertestuali. |
| address | String | Indirizzo del collegamento ipertestuale. |

### Valore di ritorno

[`Hyperlink`](../../hyperlink/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi collegamento ipertestuale usando le coordinate riga/colonna e le dimensioni.
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella. |
| totalRows | Int32 | Numero di righe in questo intervallo di collegamenti ipertestuali. |
| totalColumns | Int32 | Numero di colonne di questo intervallo di collegamenti ipertestuali. |
| address | String | Indirizzo del collegamento ipertestuale. |

### Valore di ritorno

[`Hyperlink`](../../hyperlink/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Aggiungi collegamento ipertestuale alla cella A1 con indirizzo "www.aspose.com"
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // Visualizza l'indirizzo del collegamento ipertestuale.
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // Modifica il testo visualizzato.
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startCellName | String | La cella in alto a sinistra dell'intervallo. |
| endCellName | String | La cella in basso a destra dell'intervallo. |
| address | String | Indirizzo del collegamento ipertestuale. |
| textToDisplay | String | Il testo da visualizzare per il collegamento ipertestuale specificato. |
| screenTip | String | Il testo screenTip per il collegamento ipertestuale specificato. |

### Valore di ritorno

[`Hyperlink`](../../hyperlink/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Dimostrare il metodo Add con parametri (String, String, String, String, String)
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


