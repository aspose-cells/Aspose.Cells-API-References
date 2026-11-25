---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeSaveOptions. Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null OutputFile verrà ignorato"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

Ottiene e imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, [`OutputFile`](../outputfile/) verrà ignorato.

```csharp
public Stream OutputStream { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class LowCodeSaveOptionsPropertyOutputStreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // Crea un'istanza di LowCodeSaveOptions
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // Crea uno stream di memoria per la dimostrazione
                using (MemoryStream stream = new MemoryStream())
                {
                    // Imposta la proprietà OutputStream
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // Salva utilizzando le opzioni (scriverà sul nostro stream di memoria)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // Verifica che lo stream sia stato scritto
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // Crea una nuova cartella di lavoro dallo stream per verificare il contenuto
                    Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
                    Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
                }
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

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


