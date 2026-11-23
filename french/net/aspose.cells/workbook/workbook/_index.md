---
title: "Workbook.Workbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur Workbook. Initialise une nouvelle instance de la classe Workbook"
type: docs
url: /fr/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Initialise une nouvelle instance de la classe [`Workbook`](../).

```csharp
public Workbook()
```

### Remarques

Le type de format de fichier par défaut est Xlsx. Si vous souhaitez créer d'autres types de fichiers, veuillez utiliser Workbook(FileFormatType).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur en utilisant le constructeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données aux cellules
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Enregistrez le classeur
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Initialise une nouvelle instance de la classe [`Workbook`](../).

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileFormatType | FileFormatType | Le nouveau format de fichier. |

### Remarques

Le type de format de fichier par défaut est Excel97To2003.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec le format de fichier XLSX
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Mettre des données dans la cellule A1
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

Initialise une nouvelle instance vide de la classe [`Workbook`](../) avec des options

```csharp
public Workbook(LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LoadOptions | Les options. |

### Voir aussi

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

Initialise une nouvelle instance de la classe [`Workbook`](../) et ouvre un fichier.

```csharp
public Workbook(string file)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fichier | String | Le nom du fichier. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Le chemin du répertoire des documents.
            string dataDir = "Your Document Directory";

            // Créer un classeur à partir d'un fichier Excel existant
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Afficher certaines informations de la feuille de calcul
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // Enregistrer le classeur au format MHTML
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // Créer un autre classeur à partir du fichier MHTML enregistré
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

Initialise une nouvelle instance de la classe [`Workbook`](../) et ouvre un flux.

```csharp
public Workbook(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // Créer un fichier Excel d'exemple en mémoire
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // Créer une nouvelle instance de Workbook en utilisant le constructeur Stream
                Workbook workbook = new Workbook(sampleStream);

                // Accéder à la première feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];

                // Afficher les données chargées
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // Enregistrer le classeur dans un fichier
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

Initialise une nouvelle instance de la classe [`Workbook`](../) et ouvre un fichier.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fichier | String | Le nom du fichier. |
| loadOptions | LoadOptions | Les options de chargement |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // Créer des options de chargement sans LightCellsDataHandler
            LoadOptions loadOptions = new LoadOptions();

            // Initialiser le classeur avec le chemin du fichier et les options de chargement
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Démontrer que le classeur est chargé en accédant au nombre de feuilles de calcul
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

Initialise une nouvelle instance de la classe [`Workbook`](../) et ouvre le flux.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux. |
| loadOptions | LoadOptions | Les options de chargement |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un fichier Excel d'exemple en mémoire
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // Créer LoadOptions avec des paramètres spécifiques
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // Créer une instance de Workbook en utilisant le #ctor avec Stream et LoadOptions
                Workbook workbook = new Workbook(stream, loadOptions);

                // Afficher les informations de base sur le classeur chargé
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // Accéder à la première feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // Afficher le contenu de certaines cellules si disponible
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // Créer un fichier Excel simple en mémoire à des fins de démonstration
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


