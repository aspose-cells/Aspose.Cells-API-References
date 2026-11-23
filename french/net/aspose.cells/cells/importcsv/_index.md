---
title: "Cells.ImportCSV"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Importe un fichier CSV dans les cellules"
type: docs
url: /fr/net/aspose.cells/cells/importcsv/
---
## ImportCSV(string, string, bool, int, int) {#importcsv_3}

Importe un fichier CSV dans les cellules.

```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom du fichier CSV. |
| splitter | String | Le splitter |
| convertNumericData | Boolean | Indique si la chaîne du fichier texte est convertie en données numériques. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Chemin du fichier CSV
            string csvPath = "example.csv";
            
            // Importer les données CSV en commençant à la cellule A1 (ligne 0, colonne 0)
            // Utilisation du point-virgule comme délimiteur et conversion des données numériques
            cells.ImportCSV(csvPath, ";", true, 0, 0);

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}

Importe un fichier CSV dans les cellules.

```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux du fichier CSV. |
| splitter | String | Le splitter |
| convertNumericData | Boolean | Indique si la chaîne du fichier texte est convertie en données numériques. |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer des données CSV d'exemple en mémoire
            string csvData = "Name,Age,City\nJohn,30,New York\nAlice,25,London\nBob,35,Paris";
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(csvData);
            MemoryStream csvStream = new MemoryStream(byteArray);

            try
            {
                // Appeler la méthode ImportCSV avec les paramètres Stream, String, Boolean, Int32, Int32
                cells.ImportCSV(csvStream, ",", true, 0, 0);

                Console.WriteLine("CSV data imported successfully to worksheet.");
                Console.WriteLine($"Data range: A1 to {cells.MaxDisplayRange}");

                // Enregistrez le classeur
                workbook.Save("ImportCSVFromStreamDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                csvStream?.Dispose();
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}

Importe un fichier CSV dans les cellules.

```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom du fichier CSV. |
| options | TxtLoadOptions | Les options de chargement pour la lecture du fichier texte |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des options de chargement CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            loadOptions.ConvertDateTimeData = true;
            loadOptions.ConvertNumericData = true;
            loadOptions.ParsingFormulaOnOpen = true;

            // Chemin du fichier CSV d'exemple (remplacez par le chemin réel dans votre environnement)
            string csvFilePath = "example.csv";
            
            // Importer les données CSV en commençant à la cellule A1 (ligne 0, colonne 0)
            worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}

Importe un fichier CSV dans les cellules.

```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux du fichier CSV. |
| options | TxtLoadOptions | Les options de chargement pour la lecture du fichier texte |
| firstRow | Int32 | Le numéro de ligne de la première cellule où importer. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule où importer. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection Cells
            Cells cells = worksheet.Cells;

            // Créer des données CSV d'exemple
            string csvData = "Name,Age,City\nJohn,30,New York\nJane,25,Los Angeles\nBob,35,Chicago";

            // Créer un flux mémoire avec les données CSV
            MemoryStream csvStream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData));

            try
            {
                // Créer TxtLoadOptions pour l'importation CSV
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';
                loadOptions.ConvertNumericData = true;

                // Importer les données CSV en commençant à la ligne 0, colonne 0
                cells.ImportCSV(csvStream, loadOptions, 0, 0);

                // Enregistrez le classeur
                workbook.Save("ImportCSVDemo.xlsx");

                Console.WriteLine("CSV data imported successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                // Libérer le flux
                csvStream.Dispose();
            }
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


