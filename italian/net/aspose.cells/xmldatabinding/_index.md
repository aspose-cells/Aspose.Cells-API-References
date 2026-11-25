---
title: "Classe XmlDataBinding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.XmlDataBinding. Rappresenta le informazioni di binding dei dati XML"
type: docs
url: /it/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

Rappresenta le informazioni di binding dei dati Xml.

```csharp
public class XmlDataBinding
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Ottiene l'url di origine di questo binding dei dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un oggetto elenco che utilizzerà il binding dei dati XML
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // Ottieni le informazioni del binding dei dati XML (di solito impostate durante l'importazione dei dati XML)
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // Visualizza l'URL della sorgente dati XML (proprietà di sola lettura)
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // Nota: In uno scenario reale, l'Url verrebbe impostato durante l'importazione dei dati XML
            // Ai fini della dimostrazione, mostriamo come accedere alla proprietà

            // Salva la cartella di lavoro
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


