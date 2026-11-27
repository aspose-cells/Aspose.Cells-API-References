---
title: "IFilePathProvider.GetFullName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IFilePathProvider-metod. Hämtar den fullständiga sökvägen till filen via arbetsbladets namn när arbetsbladet exporteras till HTML separat. Så att referenserna mellan arbetsbladen kan exporteras korrekt"
type: docs
url: /sv/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

Hämtar den fullständiga sökvägen till filen efter arbetsbladets namn när arbetsbladet exporteras till HTML separat. Så att referenserna mellan arbetsbladen kan exporteras korrekt.

```csharp
public string GetFullName(string sheetName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | String | Arbetsbladsnamn |

### Returvärde

den fullständiga sökvägen till filen

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en anpassad implementation av IFilePathProvider
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // Anropa GetFullName-metoden med ett bladnamn
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // Visa resultatet
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Enkel implementation som returnerar en sökväg som kombinerar bladnamnet med en katalog
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### Se även

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


