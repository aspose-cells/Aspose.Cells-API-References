---
title: "AbstractTextLoadOptions.Encoding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractTextLoadOptions. Obtient et définit l’encodage par défaut. S’applique uniquement aux fichiers csv"
type: docs
url: /fr/net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Obtient et définit l'encodage par défaut. S'applique uniquement aux fichiers csv.

```csharp
public Encoding Encoding { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Créez des données CSV d'exemple en encodage ASCII
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);

            // Chargez le classeur avec l’encodage ASCII spécifié
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            Cells cells = wb.Worksheets[0].Cells;

            // Affichez les données chargées
            Console.WriteLine($"A1: {cells[0, 0].StringValue}");
            Console.WriteLine($"B1: {cells[0, 1].StringValue}");
            Console.WriteLine($"A2: {cells[1, 0].StringValue}");
            Console.WriteLine($"B2: {cells[1, 1].IntValue}");

            // Ajoutez du texte Unicode
            cells[2, 0].PutValue("日本語のテキスト");
            
            // Enregistrer avec l'encodage UTF-8
            MemoryStream outputStream = new MemoryStream();
            wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
            
            // Afficher les premiers octets pour montrer le BOM UTF-8
            byte[] outputBytes = outputStream.ToArray();
            Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
        }
    }
}
```

### Voir aussi

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


