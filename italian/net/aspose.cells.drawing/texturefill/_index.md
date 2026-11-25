---
title: "Classe TextureFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.TextureFill. Incapsula l'oggetto che rappresenta il formato di riempimento texture"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

Incapsula l'oggetto che rappresenta il formato di riempimento a trama

```csharp
public class TextureFill : Fill
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Ottiene e imposta i dati immagine del riempimento. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Indica se l'immagine è ripetuta come texture. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Ottiene o imposta l'opzione del formato immagine. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Ottiene e imposta il tipo di formato immagine. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Ottiene e imposta la scala del formato immagine. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Ottiene o imposta l'opzione di immagine a piastrelle. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Ottiene e imposta il tipo di trama |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Ereditato da [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Ottiene il codice hash.(Ereditato da [`Fill`](../fill/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassTextureFillDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma rettangolare per dimostrare il riempimento a trama
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // Applica il riempimento a trama alla forma e ottieni l'istanza esistente di TextureFill
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // Imposta il tipo di trama incorporato
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // Configura le opzioni di piastrellatura
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // Imposta la trasparenza e la scala del riempimento
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // Salva la cartella di lavoro con il riempimento a trama applicato
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


