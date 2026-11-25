---
title: "OleObject.SetEmbeddedObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo OleObject. Imposta i dati dell'oggetto incorporato"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Imposta i dati dell'oggetto incorporato.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| linkToFile | Booleano | Indica se l'oggetto è collegato al file. Se vero, il parametro objectData viene ignorato. |
| objectData | Byte[] | I dati dell'oggetto incorporato. |
| sourceFileName | String | Il nome del file. |
| displayAsIcon | Booleano | Indica se visualizzare l'oggetto come icona. Se vero, i dati dell'immagine originale saranno coperti dall'icona. |
| label | String | L'etichetta dell'icona. Funziona solo quando displayAsIcon è vero. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un OleObject al foglio di lavoro
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Prepara i parametri per SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // Chiama SetEmbeddedObject con i parametri specificati
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // Visualizza alcune proprietà per mostrare l'effetto
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Imposta i dati dell'oggetto incorporato.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| linkToFile | Booleano | Indica se l'oggetto è collegato al file. Se vero, il parametro objectData viene ignorato. |
| objectData | Byte[] | I dati dell'oggetto incorporato. |
| sourceFileName | String | Il nome del file. |
| displayAsIcon | Booleano | Indica se visualizzare l'oggetto come icona. Se vero, i dati dell'immagine originale saranno coperti dall'icona. |
| label | String | L'etichetta dell'icona. Funziona solo quando displayAsIcon è vero. |
| updateIcon | Booleano | Indica se l'icona viene aggiornata automaticamente. |

### Osservazioni

Poiché Aspose può aggiornare tutte le icone dei file incorporati, è meglio poter aggiungere l'icona corretta impostando *updateIcon* su false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un OleObject al foglio di lavoro
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Prepara i parametri per SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // Chiama SetEmbeddedObject con i parametri specificati
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


