---
title: "WorkbookRender.ToImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookRender. Rendre le classeur complet en image Tiff vers le flux"
type: docs
url: /fr/net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

Rendre l’ensemble du classeur en tant qu’image Tiff vers un flux.

```csharp
public void ToImage(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | le flux de l'image de sortie |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithStreamDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // Configurer les options de rendu d'image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // Créer le répertoire de sortie s'il n'existe pas
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // Créer un flux de fichier pour la sortie d'image
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // Initialiser le rendu du classeur et convertir en image
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // Enregistrer le classeur original pour référence
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### Voir aussi

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

Rendre l’ensemble du classeur en tant qu’image Tiff vers un fichier.

```csharp
public void ToImage(string filename)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | String | le nom de fichier de l'image de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // Définissez les options d’image
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // Créer le rendu du classeur et enregistrer en image
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

Rendre une page donnée vers un fichier.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| fileName | String | nom de fichier de l'image de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Créer des options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // Créer le rendu du classeur
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Enregistrer chaque page en image
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

Rendre une page donnée vers un flux.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| stream | Stream | le flux de l'image de sortie |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index and Stream Demo";

            // Configurer les options de rendu d'image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            try
            {
                // Initialiser le rendu du classeur
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Obtenir l'indice de la première page (à partir de 0)
                int pageIndex = 0;

                // Créer un flux mémoire pour contenir l'image
                using (MemoryStream stream = new MemoryStream())
                {
                    // Appeler ToImage avec l'indice de page et le flux
                    renderer.ToImage(pageIndex, stream);

                    // Afficher les résultats
                    Console.WriteLine($"Page {pageIndex} rendered successfully to stream");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");
                    Console.WriteLine($"Total pages available: {renderer.PageCount}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Rendre une page donnée vers un objet Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |

### Valeur de retour

l'objet bitmap de la page

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index Demo";

            // Configurer les options de rendu d'image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

            // Créer le répertoire de sortie s'il n'existe pas
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            try
            {
                // Initialiser le rendu du classeur
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Obtenir l'indice de la première page (à partir de 0)
                int pageIndex = 0;

                // Appeler ToImage avec l'indice de page et enregistrer dans un fichier
                string imagePath = Path.Combine(outputDir, $"page_{pageIndex}.png");
                renderer.ToImage(pageIndex, imagePath);

                Console.WriteLine($"Page {pageIndex} rendered successfully to: {imagePath}");
                Console.WriteLine($"Total pages available: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


