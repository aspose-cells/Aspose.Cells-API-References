---
title: "Name.GetRefersTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Name. Ottieni il riferimento di questo Name"
type: docs
url: /it/net/aspose.cells/name/getrefersto/
---
## GetRefersTo(bool, bool) {#getrefersto}

Ottieni il riferimento di questo Name.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se il riferimento deve essere formattato come R1C1. |
| isLocal | Booleano | Indica se il riferimento deve essere formattato per impostazione locale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Crea un intervallo denominato
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Chiama GetRefersTo con formato R1C1 e ambito locale
                string refersToR1C1Local = namedRange.GetRefersTo(true, true);
                Console.WriteLine("R1C1 format with local scope: " + refersToR1C1Local);

                // Chiama GetRefersTo con formato A1 e ambito globale
                string refersToA1Global = namedRange.GetRefersTo(false, false);
                Console.WriteLine("A1 format with global scope: " + refersToA1Global);

                // Mostra i dettagli dell'intervallo denominato
                Console.WriteLine("Named range text: " + namedRange.Text);
                Console.WriteLine("Full text: " + namedRange.FullText);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("NameMethodGetRefersToDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRefersTo(bool, bool, int, int) {#getrefersto_1}

Ottieni il riferimento di questo Name basato sulla cella specificata.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se il riferimento deve essere formattato come R1C1. |
| isLocal | Booleano | Indica se il riferimento deve essere formattato per impostazione locale. |
| riga | Int32 | L'indice di riga della cella. |
| colonna | Int32 | L'indice di colonna della cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Crea un intervallo denominato
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Chiama GetRefersTo con parametri specifici (isR1C1, isLocal, row, column)
                string refersTo = namedRange.GetRefersTo(false, false, 0, 0);
                
                Console.WriteLine("Named range refers to: " + refersTo);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");

                // Modifica l'intervallo denominato in base al risultato
                if (!string.IsNullOrEmpty(refersTo))
                {
                    worksheet.Cells["B1"].PutValue("Named Range Refers To:");
                    worksheet.Cells["B2"].PutValue(refersTo);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


