---
title: "WorksheetCollection.BuiltInDocumentProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Returnerar en DocumentProperty-samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Returnerar en [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) samling som representerar alla inbyggda dokumentegenskaper i kalkylbladet.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Anmärkningar

En ny egenskap kan inte läggas till i listan över inbyggda dokumentegenskaper. Du kan bara hämta en inbyggd egenskap och ändra dess värde. Följande är listan med namn på de inbyggda egenskaperna:

Titel

Ämne

Författare

Nyckelord

Kommentarer

Mall

Senaste författare

Revisionsnummer

Programnamn

Senaste utskriftsdatum

Skapandedatum

Senaste sparningstid

Total redigeringstid

Antal sidor

Antal ord

Antal tecken

Säkerhet

Kategori

Format

Chef

Företag

Antal byte

Antal rader

Antal stycken

Antal bilder

Antal anteckningar

Antal dolda bilder

Antal multimedieklipp

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Document";
            
            Console.WriteLine("Document properties set successfully");
        }
    }
}
```

### Se även

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


