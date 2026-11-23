---
title: "Workbook.Save"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Enregistre le classeur sur le disque"
type: docs
url: /fr/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Enregistre le classeur sur le disque.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom du fichier. |
| saveFormat | SaveFormat | Le type de format d'enregistrement. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Enregistrez le classeur au format XLSX
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Enregistrez le classeur au format PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Enregistre le classeur sur le disque.

```csharp
public void Save(string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Enregistrez le classeur dans différents formats en utilisant un paramètre de chaîne
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Enregistre le classeur sur le disque.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom du fichier. |
| saveOptions | SaveOptions | Les options d'enregistrement. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Créez des options d'enregistrement HTML et configurez-les
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Enregistrez le classeur avec des options
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Enregistre le classeur dans le flux.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de fichier. |
| saveFormat | SaveFormat | Le type de format de fichier d'enregistrement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accédez à la première feuille de calcul et ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Créez un flux mémoire pour enregistrer le classeur
                using (MemoryStream stream = new MemoryStream())
                {
                    // Enregistrez le classeur dans le flux au format XLSX
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Afficher le message de succès
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Réinitialisez la position du flux pour un traitement ultérieur éventuel
                    stream.Position = 0;

                    // Enregistrez éventuellement dans un fichier pour vérification
                    using (FileStream fileStream = File.Create("StreamSaveDemo.xlsx"))
                    {
                        stream.CopyTo(fileStream);
                    }
                    Console.WriteLine("Stream content also saved to file: StreamSaveDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook to stream: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Enregistre le classeur dans le flux.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux de fichier. |
| saveOptions | SaveOptions | Les options d'enregistrement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accédez à la première feuille de calcul et ajoutez des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Créez un MemoryStream pour enregistrer le classeur
            MemoryStream stream = new MemoryStream();

            try
            {
                // Créez des SaveOptions pour le format PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Enregistrez le classeur dans le flux avec les options spécifiées
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // Réinitialiser la position du flux pour une utilisation éventuelle
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Nettoyer les ressources
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Crée la feuille de calcul résultante et la transfère au client, puis l'ouvre dans le navigateur ou le classeur MS.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| réponse | HttpResponse | Objet Response pour renvoyer la feuille de calcul au client. |
| fileName | String | Le nom du fichier créé. |
| contentDisposition | ContentDisposition | Le type de disposition du contenu. |
| saveOptions | SaveOptions | Les options d'enregistrement. |

### Remarques

Cette méthode est disponible uniquement pour les versions net4.x.

### Voir aussi

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Crée la feuille de calcul résultante et la transfère au client, puis l'ouvre dans le navigateur ou le classeur MS.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| réponse | HttpResponse | Objet Response pour renvoyer la feuille de calcul au client. |
| fileName | String | Le nom du fichier créé. |
| contentDisposition | ContentDisposition | Le type de disposition du contenu. |
| saveOptions | SaveOptions | Les options d'enregistrement. |
| enableHttpCompression | Boolean | indique si la compression http doit être utilisée |

### Remarques

Cette méthode est disponible uniquement pour les versions net4.x.

### Voir aussi

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


