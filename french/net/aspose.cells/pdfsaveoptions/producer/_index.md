---
title: "PdfSaveOptions.Producer"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PdfSaveOptions property. Obtient et définit le producteur du document pdf généré"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Obtient et définit le producteur du document pdf généré.

```csharp
public string Producer { get; set; }
```

### Remarques

Si la valeur est nulle, ou qu'une LICENCE valide n'est pas définie, la chaîne Aspose.Cells vVERSION sera utilisée.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyProducerDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul et ajouter des données d’exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // Créez les options d'enregistrement PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Définir la propriété Producer
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // Enregistrer dans le flux mémoire
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Vérifier que la propriété Producer a été définie
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine(content.Contains("/Producer (Aspose.Cells for .NET)") 
                        ? "Producer property set successfully" 
                        : "Failed to set Producer property");
                }
            }
        }
    }
}
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


