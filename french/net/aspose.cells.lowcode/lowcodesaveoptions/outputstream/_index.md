---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptions. Obtient et définit le flux (Stream) pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, OutputFile sera ignoré"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

Obtient et définit le flux (Stream) pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, [`OutputFile`](../outputfile/) sera ignoré.

```csharp
public Stream OutputStream { get; set; }
```

### Exemples

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
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // Créer une instance de LowCodeSaveOptions
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // Créer un flux mémoire pour la démonstration
                using (MemoryStream stream = new MemoryStream())
                {
                    // Définir la propriété OutputStream
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // Enregistrer en utilisant les options (écrira dans notre flux mémoire)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // Vérifier que le flux a été écrit
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // Créer un nouveau classeur à partir du flux pour vérifier le contenu
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

### Voir aussi

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


