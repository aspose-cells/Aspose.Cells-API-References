---
title: "IFilePathProvider.GetFullName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IFilePathProvider-Methode. Ermittelt den vollständigen Pfad der Datei anhand des Arbeitsblattnamens beim separaten Exportieren des Arbeitsblatts nach HTML. So können die Verweise zwischen den Arbeitsblättern korrekt exportiert werden"
type: docs
url: /de/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

Ermittelt den vollständigen Pfad der Datei anhand des Arbeitsblattnamens, wenn das Arbeitsblatt separat nach HTML exportiert wird. So können die Verweise zwischen den Arbeitsblättern korrekt exportiert werden.

```csharp
public string GetFullName(string sheetName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | String | Arbeitsblattname |

### Rückgabewert

der vollständige Pfad der Datei

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine benutzerdefinierte Implementierung von IFilePathProvider
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // Rufen Sie die GetFullName-Methode mit einem Blattnamen auf
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // Ergebnis anzeigen
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Einfache Implementierung, die einen Pfad zurückgibt, der den Blattnamen mit einem Verzeichnis kombiniert
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### Siehe auch

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


