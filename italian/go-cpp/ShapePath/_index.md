---
title: "Classe ShapePath"
linktitle: "ShapePath"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ShapePath. Incapsula l'oggetto che rappresenta shapepath in Go."
type: docs
weight: 200
url: /it/go-cpp/shapepath/
---

## ShapePath class

Rappresenta un percorso di creazione costituito da una serie di spostamenti, linee e curve che, una volta combinati, formeranno una forma geometrica.

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewShapePath](./newshapepath/) | Inizializza una nuova istanza della classe ShapePath. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetPathSegments](./getpathsegments/) | Ottiene l'elenco ShapeSegmentPathCollection |
| [GetWidthPixel](./getwidthpixel/) | Ottiene la larghezza di questo percorso in unità di pixel. |
| [SetWidthPixel](./setwidthpixel/) | Ottiene la larghezza di questo percorso in unità di pixel. |
| [GetHeightPixel](./getheightpixel/) | Ottiene l'altezza di questo percorso in unità di pixel. |
| [SetHeightPixel](./setheightpixel/) | Ottiene l'altezza di questo percorso in unità di pixel. |
| [MoveTo](./moveto/) | Avvia una nuova figura dal punto specificato senza chiudere la figura corrente. Tutti i punti successivi aggiunti al percorso sono aggiunti a questa nuova figura. Unità: Pixel. |
| [LineTo](./lineto/) | Aggiunge un segmento di linea alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità: Pixel. |
| [CubicBezierTo](./cubicbezierto/) | Aggiunge una curva Bézier cubica alla figura corrente. Il punto di partenza è il punto finale della figura corrente. Unità: Pixel. |
| [ArcTo](./arcto/) | Aggiunge un arco ellittico alla figura corrente. Il punto di partenza è il punto finale della figura corrente. |
| [Close](./close/) | Chiude la figura corrente e avvia una nuova figura. Se la figura corrente contiene una sequenza di linee e curve collegate, il metodo chiude il ciclo collegando una linea dal punto finale al punto di partenza. |
