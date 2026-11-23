---
title: "WorkbookSettings.StreamProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit le fournisseur de flux pour les ressources externes"
type: docs
url: /fr/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

Obtient et définit le fournisseur de flux pour les ressources externes.

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ResourceProvider. Cette propriété sera supprimée 12 mois plus tard à compter de juin 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider1 : IStreamProvider
    {
        private MemoryStream stream;

        public void InitStream(StreamProviderOptions options)
        {
            stream = new MemoryStream();
            options.Stream = stream;
        }

        public void CloseStream(StreamProviderOptions options)
        {
            stream.Close();
            Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
        }
    }

    public class WorkbookSettingsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Afficher la valeur actuelle du StreamProvider
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // Définir un fournisseur de flux personnalisé
            settings.StreamProvider = new CustomStreamProvider1();

            // Ajouter des données pour démontrer l'utilisation du flux
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // Enregistrer le classeur - cela déclenchera le fournisseur de flux
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // Réinitialiser le fournisseur de flux
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### Voir aussi

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


