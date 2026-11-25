---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo HtmlTableLoadOptionCollection. Aggiunge un HtmlTableLoadOption a questa collezione"
type: docs
url: /it/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

Aggiunge un HtmlTableLoadOption a questa collezione.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | HtmlTableLoadOption | un HtmlTableLoadOption |

### Valore di ritorno

l'indice dell'elemento aggiunto

### Osservazioni

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo AddTableLoadOption(). Questo metodo sarà rimosso tra 6 mesi a partire da dicembre 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Aggiungi opzioni di caricamento della tabella
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Carica la cartella di lavoro con opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Salva l'output
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

Aggiungi un HtmlTableLoadOption all'elenco.

```csharp
public int Add(int tableIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableIndex | Int32 | Indice della tabella |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accedi all'istanza di HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Aggiungi una nuova HtmlTableLoadOption per indice tabella
            int index = tableLoadOptions.Add(0);

            // Accedi all'HtmlTableLoadOption aggiunto
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // Crea una cartella di lavoro e carica HTML con opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

Aggiungi un HtmlTableLoadOption all'elenco.

```csharp
public int Add(string tableId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableId | String | ID della tabella |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accedi all'istanza di HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Aggiungi una nuova HtmlTableLoadOption per ID tabella
            int index = tableLoadOptions.Add("mainTable");

            // Accedi all'HtmlTableLoadOption aggiunto
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // Crea una cartella di lavoro e carica HTML con opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

Aggiungi un HtmlTableLoadOption all'elenco.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableIndex | Int32 | Indice della tabella |
| targetSheetIndex | Int32 | L'indice di destinazione del foglio di lavoro in Excel |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Aggiungi tabelle per indice con indice del foglio di destinazione
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // Carica il file HTML con le opzioni specificate
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

Aggiungi un HtmlTableLoadOption all'elenco.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableId | String | ID della tabella |
| targetSheetIndex | Int32 | L'indice di destinazione del foglio di lavoro in Excel |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accedi all'istanza di HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Aggiungi una nuova HtmlTableLoadOption per ID tabella e indice foglio di destinazione
            int index = tableLoadOptions.Add("tableId", 1);

            // Crea una cartella di lavoro e carica HTML con opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

Aggiungi un HtmlTableLoadOption all'elenco.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableIndex | Int32 | Indice della tabella |
| targetSheetIndex | Int32 | L'indice di destinazione del foglio di lavoro in Excel |
| originalSheetIndex | Int32 | L'indice originale del foglio di lavoro nell'HTML |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Accedi a HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Aggiungi una tabella con indice 1, indice del foglio di destinazione 1 e indice del foglio originale 0
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // Crea una cartella di lavoro e carica HTML con opzioni
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

Aggiungi un HtmlTableLoadOption all'elenco.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableId | String | ID della tabella |
| targetSheetIndex | Int32 | L'indice di destinazione del foglio di lavoro in Excel |
| originalSheetIndex | Int32 | L'indice originale del foglio di lavoro nell'HTML |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Dimostra il metodo Add con parametri (String, Int32, Int32)
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // Carica il file HTML (sostituisci con il percorso reale del file)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


