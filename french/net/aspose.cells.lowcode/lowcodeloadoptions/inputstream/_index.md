---
title: "LowCodeLoadOptions.InputStream"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeLoadOptions. Obtient et définit le flux du modèle"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

Obtient et définit le flux du modèle.

```csharp
public Stream InputStream { get; set; }
```

### Remarques

Lors de la définition d'un flux non nul pour cette propriété, la valeur précédemment définie pour [`InputFile`](../inputfile/) sera ignorée.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // Créez des données d'exemple dans un flux mémoire
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // Créez des options de chargement avec InputStream
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // Créez un nouveau classeur en utilisant le flux
                using (Workbook workbook = new Workbook(stream))
                {
                    // Accéder à la première feuille de calcul
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // Démontrez que le contenu a été chargé
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


