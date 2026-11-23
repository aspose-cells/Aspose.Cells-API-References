---
title: "HtmlSaveOptions.Encoding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Si non définie, utilisez Encoding.UTF8 comme type d'encodage par défaut"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

Si non défini, utilisez Encoding.UTF8 comme type d'encodage par défaut.

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
    public class HtmlSaveOptionsPropertyEncodingDemo
    {
        private class SheetStreamProvider : IStreamProvider
        {
            private readonly MemoryStream _sheet1Stream;
            private readonly MemoryStream _sheet2Stream;
            private int _currentIndex = 0;

            public SheetStreamProvider(MemoryStream sheet1Stream, MemoryStream sheet2Stream)
            {
                _sheet1Stream = sheet1Stream;
                _sheet2Stream = sheet2Stream;
            }

            public void InitStream(StreamProviderOptions options)
            {
                // Initialisation si nécessaire
            }

            public Stream GetStream(string sheetName)
            {
                return _currentIndex++ == 0 ? _sheet1Stream : _sheet2Stream;
            }

            public void CloseStream(StreamProviderOptions options)
            {
                options.Stream?.Flush();
            }
        }

        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données d'exemple aux feuilles de calcul
            workbook.Worksheets[0].Cells[0, 0].PutValue("Sample content in Sheet1");
            workbook.Worksheets.Add("Sheet2").Cells[0, 0].PutValue("Sample content in Sheet2");

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir l'encodage sur UTF8
            saveOptions.Encoding = Encoding.UTF8;

            // Créer des flux mémoire pour la sortie
            using (MemoryStream sheet1Stream = new MemoryStream())
            using (MemoryStream sheet2Stream = new MemoryStream())
            {
                // Créer un fournisseur de flux pour gérer plusieurs feuilles
                SheetStreamProvider streamProvider = new SheetStreamProvider(sheet1Stream, sheet2Stream);
                saveOptions.StreamProvider = streamProvider;

                // Enregistrer le classeur avec les options HTML
                workbook.Save(new MemoryStream(), saveOptions);

                // Vérifier que le contenu a été enregistré avec l'encodage UTF8
                string sheet1Content = Encoding.UTF8.GetString(sheet1Stream.ToArray());
                string sheet2Content = Encoding.UTF8.GetString(sheet2Stream.ToArray());

                Console.WriteLine("Sheet1 content contains text: " + 
                    sheet1Content.Contains("Sample content in Sheet1"));
                Console.WriteLine("Sheet2 content contains text: " + 
                    sheet2Content.Contains("Sample content in Sheet2"));
            }
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


