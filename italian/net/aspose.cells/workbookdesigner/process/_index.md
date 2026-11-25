---
title: "WorkbookDesigner.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookDesigner. Elabora i marcatori intelligenti e popola i valori dell'origine dati"
type: docs
url: /it/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Elabora gli smart marker e popola i valori dell'origine dati.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo da elaborare |
| isPreserved | Booleano | True se il marcatore intelligente non riconosciuto è preservato. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare i marcatori intelligenti di Range. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea dati di esempio nelle celle
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // Crea il designer di cartella di lavoro
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // Crea origine dati JSON
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // Elabora intervallo specifico con marcatori intelligenti
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // Elabora l'intervallo (true = elabora solo questo intervallo)
            designer.Process(range, true);
            
            // Salva il risultato
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Elabora gli smart marker e popola i valori dell'origine dati.

```csharp
public void Process()
```

### Esempi

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro da file modello
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Prepara la fonte dati
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // Imposta la fonte dati ed elabora
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Elabora gli smart marker e popola i valori dell'origine dati.

```csharp
public void Process(bool isPreserved)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isPreserved | Booleano | True se il marcatore intelligente non riconosciuto è preservato. |

### Esempi

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // Inizializza la cartella di lavoro e carica il modello
            Workbook workbook = new Workbook("example.xlsx");
            
            // Crea dati di esempio direttamente invece di caricarli da JSON
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // Configura i marcatori intelligenti
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // Prepara le fonti dati
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // Elabora il designer della cartella di lavoro
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // Elabora con parametro booleano
            designer.Process(true);
            
            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }

    // Classi di dati di esempio
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Elabora gli smart marker e popola i valori dell'origine dati.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | Indice del foglio di lavoro. |
| isPreserved | Booleano | True se il marcatore intelligente non riconosciuto è preservato. |

### Osservazioni

Questo metodo funziona a livello di foglio di lavoro.

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file sorgente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Esporta dati dal foglio di lavoro al DataTable
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // Crea il designer della cartella di lavoro e imposta la fonte dati
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // Elabora il designer con i parametri (Int32, Boolean)
            designer.Process(0, true);

            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


