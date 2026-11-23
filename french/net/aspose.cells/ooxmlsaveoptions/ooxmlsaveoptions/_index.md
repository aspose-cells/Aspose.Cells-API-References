---
title: "OoxmlSaveOptions.OoxmlSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur OoxmlSaveOptions. Crée les options pour enregistrer un fichier Office Open XML"
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Crée les options pour enregistrer le fichier Office Open XML.

```csharp
public OoxmlSaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Démontrer le constructeur OoxmlSaveOptions
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            
            // Enregistrer le classeur avec les options OOXML
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML options.");
        }
    }
}
```

### Voir aussi

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Crée les options pour enregistrer le fichier Office Open XML.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | Le format de fichier. Il doit être l'un des types suivants : Xlsx, Xltx, Xlam, Xlsm ou Xltm, sinon le format enregistré sera automatiquement défini sur Xlsx. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            try
            {
                // Créer OoxmlSaveOptions avec le paramètre SaveFormat
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                
                // Définir certaines propriétés des options d'enregistrement
                saveOptions.ExportCellName = true;
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                
                Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
                
                // Enregistrer le classeur avec les options spécifiées
                workbook.Save("OoxmlSaveOptionsCtorDemo.xlsx", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating OoxmlSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


