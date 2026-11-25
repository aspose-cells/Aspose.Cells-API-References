---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Aggiunge una funzione add-in alla cartella di lavoro"
type: docs
url: /it/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Aggiunge la funzione addin nella cartella di lavoro

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| addInFile | String | il file contiene le funzioni add-in |
| functionName | String | il nome della funzione add-in |
| lib | Booleano | indica se il file add-in fornito si trova nella directory o sottodirectory della libreria Add-In della cartella di lavoro. Questa opzione ha effetto e fa differenza quando il addInFile fornito è un percorso relativo: true indica che il percorso è relativo alla libreria Add-In e false indica che il percorso è relativo a questa cartella di lavoro. |

### Valore di ritorno

ID dei dati che contengono la funzione add-in fornita

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Ottieni il primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            
            // Imposta percorsi di file di esempio (devono esistere nel tuo ambiente)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // Registra funzioni add-in con parametri diversi
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // Utilizza le funzioni registrate nelle celle
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // Salva la cartella di lavoro
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Aggiunge la funzione addin nella cartella di lavoro

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| id | Int32 | ID dei dati che contengono le funzioni add-in, può essere ottenuto dalla prima chiamata di `RegisterAddInFunction` per lo stesso file add-in. |
| functionName | String | il nome della funzione add-in |

### Valore di ritorno

URL del file add-in che contiene le funzioni add-in

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Registra la prima funzione add-in e ottieni il suo ID
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // Registra la seconda funzione add-in usando lo stesso ID
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Usa le funzioni registrate nelle formule
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // Salva la cartella di lavoro
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


