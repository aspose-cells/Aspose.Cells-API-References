---
title: "ImageConverter.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ImageConverter. Convertit le fichier modèle en images"
type: docs
url: /fr/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Convertit le fichier modèle en images.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | String | Le fichier modèle à convertir en images. |
| resultFile | String | Le fichier résultant (modèle de nom) pour les images générées. |

### Remarques

Les fichiers de sortie seront construits à partir du fichier résultat spécifié en ajoutant le numéro de séquence de la feuille et la partie découpée. Par exemple, si le fichier de sortie spécifié est Image.png, alors les fichiers image générés seront Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et le remplir avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // Enregistrer comme fichier modèle pour le traitement
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // Convertir le modèle en images en utilisant les paramètres (String, String)
                ImageConverter.Process("Template.xlsx", "OutputSheet.png");

                Console.WriteLine("Process method executed successfully. Generated image(s) from spreadsheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image conversion: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convertit le fichier modèle en images

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options de sortie et d'enregistrement |

### Remarques

Lors de la conversion en image d'un format qui prend en charge plusieurs pages (comme le tiff), le [`OutputFile`](../../lowcodesaveoptions/outputfile/) ou le [`OutputStream`](../../lowcodesaveoptions/outputstream/) spécifié sera utilisé directement pour l'image résultante. Pour les autres types d'image, si les options d'enregistrement ont spécifié un Stream comme sortie, alors toutes les images résultantes seront enregistrées dans le même Stream. Sinon, les fichiers de sortie seront construits à partir du fichier de sortie spécifié des options d'enregistrement en ajoutant le numéro de séquence de la feuille et la partie découpée. Par exemple, si le fichier de sortie spécifié est Image.png, alors les fichiers image générés seront Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            try
            {
                // Initialiser LowCodeLoadOptions avec un fichier modèle
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // Initialiser LowCodeSaveOptions avec le répertoire de sortie
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // Exécuter la méthode Process avec les paramètres spécifiés
                ImageConverter.Process(loadOptions, saveOptions);
                
                Console.WriteLine("Spreadsheet converted to images successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during processing: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Convertit le fichier modèle en images

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options d'enregistrement. Sa sortie ([`OutputFile`](../../lowcodesaveoptions/outputfile/) ou [`OutputStream`](../../lowcodesaveoptions/outputstream/)) n'a aucun effet car toutes les sorties seront spécifiées par le paramètre \"provider\". |
| provider | AbstractLowCodeSaveOptionsProvider | Fournisseur des options d'enregistrement pour enregistrer les images générées |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
            const string templatePath = "SampleTemplate.xlsx";
            const string outputDir = "Output/";
            
            // Créer un modèle d'exemple
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // Initialiser les options de chargement
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // Configurer les options d'enregistrement en utilisant LowCodeImageSaveOptions
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // Appeler la méthode statique Process
                ImageConverter.Process(loadOptions, saveOptions, provider);
                Console.WriteLine($"Generated PNG images in: {Path.GetFullPath(outputDir)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Processing failed: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string path)
        {
            using (Workbook wb = new Workbook())
            {
                Worksheet sheet = wb.Worksheets[0];
                sheet.Cells["A1"].PutValue("LowCode Process Demo");
                sheet.Cells["B3"].PutValue(DateTime.Now.ToString());
                wb.Save(path, SaveFormat.Xlsx);
            }
        }

        private class DynamicSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            private readonly LowCodeImageSaveOptions _baseOptions; // Corrected type

            public DynamicSaveOptionsProvider(LowCodeImageSaveOptions options)
            {
                _baseOptions = options;
            }

            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Accéder aux propriétés de résolution depuis LowCodeImageSaveOptions
                if (partInfo.SheetIndex == 0)
                {
                    _baseOptions.ImageOptions.HorizontalResolution = 300;
                    _baseOptions.ImageOptions.VerticalResolution = 300;
                }
                return _baseOptions;
            }
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


