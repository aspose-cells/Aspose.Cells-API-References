---
title: "LowCodeLoadOptions.InputFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeLoadOptions. Ottiene e imposta il percorso del file, se necessario, del modello"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

Ottiene e imposta il file (con percorso se necessario) del modello.

```csharp
public string InputFile { get; set; }
```

### Osservazioni

Quando si imposta un percorso non nullo e non vuoto per questa proprietà, il valore precedentemente impostato per [`InputStream`](../inputstream/) verrà ignorato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // Crea e salva un file modello di esempio
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // Inizializza LowCodeLoadOptions e dimostra la proprietà InputFile
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // Imposta la proprietà InputFile per utilizzare il nostro modello
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // Carica la cartella di lavoro usando il file modello specificato
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // Modifica il modello caricato
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // Salva la cartella di lavoro modificata
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


