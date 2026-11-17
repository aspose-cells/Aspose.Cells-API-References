---
title: "Classe SmartArtShape"
linktitle: "SmartArtShape"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe SmartArtShape. Incapsula l'oggetto che rappresenta smartartshape in Go."
type: docs
weight: 200
url: /it/go-cpp/smartartshape/
---

## SmartArtShape class

Rappresenta lo smart art.

```go

type SmartArtShape struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewSmartArtShape](./newsmartartshape/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetResultOfSmartArt](./getresultofsmartart/) | Conversione di SmartArt in forme raggruppate. |
| [GetMacroName](./getmacroname/) | Ottiene e imposta il nome della macro. |
| [SetMacroName](./setmacroname/) | Ottiene e imposta il nome della macro. |
| [IsEquation](./isequation/) | Indica se la forma contiene solo un'equazione. |
| [IsSmartArt](./issmartart/) | Indica se la forma è un smart art. |
| [ToFrontOrBack](./tofrontorback/) | Porta la forma in primo piano o invia la forma sullo sfondo. |
| [GetZOrderPosition](./getzorderposition/) | Restituisce la posizione di una forma nell'ordine Z. |
| [SetZOrderPosition](./setzorderposition/) | Restituisce la posizione di una forma nell'ordine Z. |
| [GetName](./getname/) | Ottiene e imposta il nome della forma. |
| [SetName](./setname/) | Ottiene e imposta il nome della forma. |
| [GetAlternativeText](./getalternativetext/) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Shape. |
| [SetAlternativeText](./setalternativetext/) | Restituisce o imposta la stringa di testo descrittiva (alternativa) dell'oggetto Shape. |
| [GetTitle](./gettitle/) | Specifica il titolo (didascalia) dell'oggetto forma corrente. |
| [SetTitle](./settitle/) | Specifica il titolo (didascalia) dell'oggetto forma corrente. |
| [GetLine](./getline/) | Ottiene lo stile della linea |
| [GetFill](./getfill/) | Restituisce un oggetto FillFormat che contiene le proprietà di formattazione di riempimento per la forma specificata. |
| [GetShadowEffect](./getshadoweffect/) | Rappresenta un oggetto Drawing.ShadowEffect che specifica l'effetto ombra per l'elemento del grafico o la forma. |
| [GetReflection](./getreflection/) | Rappresenta un oggetto ReflectionEffect che specifica l'effetto di riflessione per l'elemento del grafico o la forma. |
| [GetGlow](./getglow/) | Rappresenta un oggetto GlowEffect che specifica l'effetto di bagliore per l'elemento del grafico o la forma. |
| [GetSoftEdges](./getsoftedges/) | Ottiene e imposta il raggio della sfocatura da applicare ai bordi, in unità di punti. |
| [SetSoftEdges](./setsoftedges/) | Ottiene e imposta il raggio della sfocatura da applicare ai bordi, in unità di punti. |
| [GetThreeDFormat](./getthreedformat/) | Ottiene e imposta il formato 3D della forma. |
| [GetFormatPicture](./getformatpicture/) | Ottiene e imposta le opzioni del formato immagine. |
| [IsHidden](./ishidden/) | Indica se l'oggetto è visibile. |
| [SetIsHidden](./setishidden/) | Indica se l'oggetto è visibile. |
| [IsAspectRatioLocked](./isaspectratiolocked/) | True indica che il rapporto d'aspetto della forma è bloccato. |
| [SetIsAspectRatioLocked](./setisaspectratiolocked/) | True indica che il rapporto d'aspetto della forma è bloccato. |
| [GetLockedProperty](./getlockedproperty/) | Ottiene il valore della proprietà locked. |
| [SetLockedProperty](./setlockedproperty/) | Imposta la proprietà locked. |
| [GetRotationAngle](./getrotationangle/) | Ottiene e imposta la rotazione della forma. |
| [SetRotationAngle](./setrotationangle/) | Ottiene e imposta la rotazione della forma. |
| [AddHyperlink](./addhyperlink/) | Aggiunge un collegamento ipertestuale alla forma. |
| [RemoveHyperlink](./removehyperlink/) | Rimuove il collegamento ipertestuale della forma. |
| [GetHyperlink](./gethyperlink/) | Ottiene il collegamento ipertestuale della forma. |
| [MoveToRange](./movetorange/) | Sposta la forma in un intervallo specificato. |
| [AlignTopRightCorner](./aligntoprightcorner/) | Sposta l'immagine nell'angolo in alto a destra. |
| [GetId](./getid/) | Ottiene l'identificatore di questa forma. |
| [GetSpid](./getspid/) | Specifica un identificatore di stringa opzionale che un'applicazione può utilizzare per identificare la forma specifica. |
| [GetSpt](./getspt/) | Specifica un numero opzionale che un'applicazione può utilizzare per associare la forma specifica a un tipo di forma definito. |
| [GetWorksheet](./getworksheet/) | Ottiene l'oggetto Aspose.Cells.Worksheet che contiene questa forma. |
| [IsGroup](./isgroup/) | Indica se questa forma è una forma di gruppo. |
| [IsInGroup](./isingroup/) | Indica se la forma è raggruppata. |
| [IsWordArt](./iswordart/) | Indica se questa forma è un WordArt. |
| [GetTextEffect](./gettexteffect/) | Restituisce un oggetto TextEffectFormat che contiene le proprietà di formattazione degli effetti di testo per la forma specificata. Si applica agli oggetti Shape che rappresentano WordArt. |
| [IsLocked](./islocked/) | True indica che l'oggetto non può essere modificato quando il foglio è protetto. Nota che questo valore è significativo solo se il foglio di lavoro o gli oggetti nel foglio di lavoro sono protetti. |
| [SetIsLocked](./setislocked/) | True indica che l'oggetto non può essere modificato quando il foglio è protetto. Nota che questo valore è significativo solo se il foglio di lavoro o gli oggetti nel foglio di lavoro sono protetti. |
| [IsPrintable](./isprintable/) | Indica se l'oggetto è stampabile. Se False, questa forma non verrà stampata durante la stampa. |
| [SetIsPrintable](./setisprintable/) | Indica se l'oggetto è stampabile. Se False, questa forma non verrà stampata durante la stampa. |
| [GetMsoDrawingType](./getmsodrawingtype/) | Ottiene il tipo di disegno. |
| [GetAutoShapeType](./getautoshapetype/) | Ottiene e imposta il tipo di forma automatica. |
| [SetAutoShapeType](./setautoshapetype/) | Ottiene e imposta il tipo di forma automatica. |
| [GetAnchorType](./getanchortype/) | Ottiene e imposta il tipo del segnaposto di ancoraggio della forma. |
| [SetAnchorType](./setanchortype/) | Ottiene e imposta il tipo del segnaposto di ancoraggio della forma. |
| [GetPlacement](./getplacement/) | Rappresenta il modo in cui l'oggetto di disegno è ancorato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro. |
| [SetPlacement](./setplacement/) | Rappresenta il modo in cui l'oggetto di disegno è ancorato alle celle sottostanti. La proprietà controlla il posizionamento di un oggetto su un foglio di lavoro. |
| [GetUpperLeftRow](./getupperleftrow/) | Rappresenta l'indice della riga superiore. |
| [SetUpperLeftRow](./setupperleftrow/) | Rappresenta l'indice della riga superiore. |
| [GetUpperDeltaY](./getupperdeltay/) | Ottiene o imposta lo spostamento verticale della forma dalla riga dell'angolo superiore sinistro. |
| [SetUpperDeltaY](./setupperdeltay/) | Ottiene o imposta lo spostamento verticale della forma dalla riga dell'angolo superiore sinistro. |
| [GetUpperLeftColumn](./getupperleftcolumn/) | Rappresenta l'indice della colonna dell'angolo superiore sinistro. |
| [SetUpperLeftColumn](./setupperleftcolumn/) | Rappresenta l'indice della colonna dell'angolo superiore sinistro. |
| [GetUpperDeltaX](./getupperdeltax/) | Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro. |
| [SetUpperDeltaX](./setupperdeltax/) | Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo superiore sinistro. |
| [GetLowerRightRow](./getlowerrightrow/) | Rappresenta l'indice della riga dell'angolo inferiore destro. |
| [SetLowerRightRow](./setlowerrightrow/) | Rappresenta l'indice della riga dell'angolo inferiore destro. |
| [GetLowerDeltaY](./getlowerdeltay/) | Ottiene o imposta lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. |
| [SetLowerDeltaY](./setlowerdeltay/) | Ottiene o imposta lo spostamento verticale della forma dalla riga dell'angolo inferiore destro. |
| [GetLowerRightColumn](./getlowerrightcolumn/) | Rappresenta l'indice della colonna dell'angolo inferiore destro. |
| [SetLowerRightColumn](./setlowerrightcolumn/) | Rappresenta l'indice della colonna dell'angolo inferiore destro. |
| [GetLowerDeltaX](./getlowerdeltax/) | Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. |
| [SetLowerDeltaX](./setlowerdeltax/) | Ottiene o imposta lo spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro. |
| [GetRight](./getright/) | Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel. |
| [SetRight](./setright/) | Rappresenta la larghezza dello spostamento orizzontale della forma dalla colonna dell'angolo inferiore destro, in unità di pixel. |
| [GetBottom](./getbottom/) | Rappresenta la larghezza dello spostamento verticale della forma dalla riga dell'angolo inferiore, in unità di pixel. |
| [SetBottom](./setbottom/) | Rappresenta la larghezza dello spostamento verticale della forma dalla riga dell'angolo inferiore, in unità di pixel. |
| [GetWidth](./getwidth/) | Rappresenta la larghezza della forma, in unità di pixel. |
| [SetWidth](./setwidth/) | Rappresenta la larghezza della forma, in unità di pixel. |
| [GetWidthInch](./getwidthinch/) | Rappresenta la larghezza della forma, in unità di pollici. |
| [SetWidthInch](./setwidthinch/) | Rappresenta la larghezza della forma, in unità di pollici. |
| [GetWidthPt](./getwidthpt/) | Rappresenta la larghezza della forma, in unità di punti. |
| [SetWidthPt](./setwidthpt/) | Rappresenta la larghezza della forma, in unità di punti. |
| [GetWidthCM](./getwidthcm/) | Rappresenta la larghezza della forma, in unità di centimetri. |
| [SetWidthCM](./setwidthcm/) | Rappresenta la larghezza della forma, in unità di centimetri. |
| [GetHeight](./getheight/) | Rappresenta l'altezza della forma, in unità di pixel. |
| [SetHeight](./setheight/) | Rappresenta l'altezza della forma, in unità di pixel. |
| [GetHeightInch](./getheightinch/) | Rappresenta l'altezza della forma, in unità di pollici. |
| [SetHeightInch](./setheightinch/) | Rappresenta l'altezza della forma, in unità di pollici. |
| [GetHeightPt](./getheightpt/) | Rappresenta l'altezza della forma, in unità di punti. |
| [SetHeightPt](./setheightpt/) | Rappresenta l'altezza della forma, in unità di punti. |
| [GetHeightCM](./getheightcm/) | Rappresenta l'altezza della forma, in unità di centimetri. |
| [SetHeightCM](./setheightcm/) | Rappresenta l'altezza della forma, in unità di centimetri. |
| [GetLeft](./getleft/) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| [SetLeft](./setleft/) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| [GetLeftInch](./getleftinch/) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici. |
| [SetLeftInch](./setleftinch/) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pollici. |
| [GetLeftCM](./getleftcm/) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri. |
| [SetLeftCM](./setleftcm/) | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di centimetri. |
| [GetTop](./gettop/) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel. |
| [SetTop](./settop/) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pixel. |
| [GetTopInch](./gettopinch/) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici. |
| [SetTopInch](./settopinch/) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di pollici. |
| [GetTopCM](./gettopcm/) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri. |
| [SetTopCM](./settopcm/) | Rappresenta lo spostamento verticale della forma dalla sua riga superiore, in unità di centimetri. |
| [GetTopToCorner](./gettoptocorner/) | Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [SetTopToCorner](./settoptocorner/) | Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro, in unità di pixel. |
| [GetLeftToCorner](./getlefttocorner/) | Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro. |
| [SetLeftToCorner](./setlefttocorner/) | Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro. |
| [GetX](./getx/) | Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro,in unità di pixel. |
| [SetX](./setx/) | Ottiene e imposta lo spostamento orizzontale della forma dal bordo sinistro del foglio di lavoro,in unità di pixel. |
| [GetY](./gety/) | Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro,in unità di pixel. |
| [SetY](./sety/) | Ottiene e imposta lo spostamento verticale della forma dal bordo superiore del foglio di lavoro,in unità di pixel. |
| [GetWidthScale](./getwidthscale/) | Ottiene e imposta la scala di larghezza, in unità di percentuale della larghezza originale dell'immagine.Se la forma non è un'immagine ,la proprietà WidthScale restituisce solo 100; |
| [SetWidthScale](./setwidthscale/) | Ottiene e imposta la scala di larghezza, in unità di percentuale della larghezza originale dell'immagine.Se la forma non è un'immagine ,la proprietà WidthScale restituisce solo 100; |
| [GetHeightScale](./getheightscale/) | Ottiene e imposta la scala di altezza,in unità di percentuale dell'altezza originale dell'immagine.Se la forma non è un'immagine ,la proprietà HeightScale restituisce solo 100; |
| [SetHeightScale](./setheightscale/) | Ottiene e imposta la scala di altezza,in unità di percentuale dell'altezza originale dell'immagine.Se la forma non è un'immagine ,la proprietà HeightScale restituisce solo 100; |
| [GetTopInShape](./gettopinshape/) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore,in unità di 1/4000 dell'altezza della forma genitore. |
| [SetTopInShape](./settopinshape/) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore,in unità di 1/4000 dell'altezza della forma genitore. |
| [GetLeftInShape](./getleftinshape/) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma genitore,in unità di 1/4000 della larghezza della forma genitore. |
| [SetLeftInShape](./setleftinshape/) | Rappresenta lo spostamento orizzontale della forma dal bordo sinistro della forma genitore,in unità di 1/4000 della larghezza della forma genitore. |
| [GetWidthInShape](./getwidthinshape/) | Rappresenta la larghezza della forma, in unità di 1/4000 della forma genitore. |
| [SetWidthInShape](./setwidthinshape/) | Rappresenta la larghezza della forma, in unità di 1/4000 della forma genitore. |
| [GetHeightInShape](./getheightinshape/) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore.. |
| [SetHeightInShape](./setheightinshape/) | Rappresenta lo spostamento verticale della forma dal bordo superiore della forma genitore, in unità di 1/4000 dell'altezza della forma genitore.. |
| [GetGroup](./getgroup/) | Ottiene la forma di gruppo che contiene questa forma. |
| [GetType](./gettype/) | Ottiene il tipo di forma automatica. |
| [GetHasLine](./gethasline/) | Ottiene e imposta se il bordo della forma è visibile. |
| [SetHasLine](./sethasline/) | Ottiene e imposta se il bordo della forma è visibile. |
| [IsFilled](./isfilled/) | Indica se il formato di riempimento è visibile. |
| [SetIsFilled](./setisfilled/) | Indica se il formato di riempimento è visibile. |
| [IsFlippedHorizontally](./isflippedhorizontally/) | Ottiene e imposta se la forma è capovolta orizzontalmente . |
| [SetIsFlippedHorizontally](./setisflippedhorizontally/) | Ottiene e imposta se la forma è capovolta orizzontalmente . |
| [IsFlippedVertically](./isflippedvertically/) | Ottiene e imposta se la forma è capovolta verticalmente. |
| [SetIsFlippedVertically](./setisflippedvertically/) | Ottiene e imposta se la forma è capovolta verticalmente. |
| [GetActualLowerRightRow](./getactuallowerrightrow/) | Ottieni la riga inferiore reale. |
| [GetConnectionPoints](./getconnectionpoints/) | Ottieni i punti di connessione |
| [ToImage_ImageType](./toimage_imagetype/) | Crea l'immagine della forma e la salva in uno stream nel formato specificato. |
| [GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | Indica se la forma è relativa alle dimensioni dell'immagine originale. |
| [SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | Indica se la forma è relativa alle dimensioni dell'immagine originale. |
| [GetLinkedCell](./getlinkedcell/) | Ottiene o imposta l'intervallo del foglio di lavoro collegato al valore del controllo. |
| [SetLinkedCell_String](./setlinkedcell_string/) | Ottiene o imposta l'intervallo del foglio di lavoro collegato al valore del controllo. |
| [GetInputRange](./getinputrange/) | Ottiene o imposta l'intervallo del foglio di lavoro usato per riempire la casella combinata specificata. |
| [SetInputRange_String](./setinputrange_string/) | Ottiene o imposta l'intervallo del foglio di lavoro usato per riempire la casella combinata specificata. |
| [UpdateSelectedValue](./updateselectedvalue/) | Aggiorna il valore selezionato con il valore della cella collegata. |
| [GetTextShapeType](./gettextshapetype/) | Ottiene e imposta il tipo di forma di testo predefinito. |
| [SetTextShapeType](./settextshapetype/) | Ottiene e imposta il tipo di forma di testo predefinito. |
| [GetTextBody](./gettextbody/) | Ottiene e imposta la configurazione del testo della forma. |
| [GetFont](./getfont/) | Rappresenta il carattere della forma. |
| [SetFont](./setfont/) | Rappresenta il carattere della forma. |
| [GetTextOptions](./gettextoptions/) | Rappresenta le opzioni di testo della forma. |
| [SetTextOptions](./settextoptions/) | Rappresenta le opzioni di testo della forma. |
| [CalculateTextSize](./calculatetextsize/) | Ricalcola l'area di testo |
| [GetText](./gettext/) | Ottiene e imposta il testo di questa forma. |
| [SetText](./settext/) | Ottiene e imposta il testo di questa forma. |
| [IsRichText](./isrichtext/) | Indica se il testo è rich text. |
| [GetHtmlText](./gethtmltext/) | Ottiene e imposta la stringa HTML che contiene dati e alcuni formati in questa casella di testo. |
| [SetHtmlText](./sethtmltext/) | Ottiene e imposta la stringa HTML che contiene dati e alcuni formati in questa casella di testo. |
| [FormatCharacters](./formatcharacters/) | Formatta alcuni caratteri con l'impostazione del carattere. |
| [Characters](./characters/) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri nel testo. |
| [GetRichFormattings](./getrichformattings/) | Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo. |
| [GetTextVerticalOverflow](./gettextverticaloverflow/) | Ottiene e imposta il tipo di overflow verticale del testo della forma che contiene testo. |
| [SetTextVerticalOverflow](./settextverticaloverflow/) | Ottiene e imposta il tipo di overflow verticale del testo della forma che contiene testo. |
| [GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | Ottiene e imposta il tipo di overflow orizzontale del testo della forma che contiene testo. |
| [SetTextHorizontalOverflow](./settexthorizontaloverflow/) | Ottiene e imposta il tipo di overflow orizzontale del testo della forma che contiene testo. |
| [IsTextWrapped](./istextwrapped/) | Ottiene e imposta il tipo di avvolgimento del testo della forma che contiene testo. |
| [SetIsTextWrapped](./setistextwrapped/) | Ottiene e imposta il tipo di avvolgimento del testo della forma che contiene testo. |
| [GetTextOrientationType](./gettextorientationtype/) | Ottiene e imposta il tipo di orientamento del testo della forma. |
| [SetTextOrientationType](./settextorientationtype/) | Ottiene e imposta il tipo di orientamento del testo della forma. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Ottiene e imposta il tipo di allineamento orizzontale del testo della forma. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Ottiene e imposta il tipo di allineamento orizzontale del testo della forma. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Ottiene e imposta il tipo di allineamento verticale del testo della forma. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Ottiene e imposta il tipo di allineamento verticale del testo della forma. |
| [GetTextDirection](./gettextdirection/) | Ottiene/Imposta la direzione del flusso di testo per questo oggetto. |
| [SetTextDirection](./settextdirection/) | Ottiene/Imposta la direzione del flusso di testo per questo oggetto. |
| [GetTextBoxOptions](./gettextboxoptions/) | Ottiene le informazioni di testo nella forma |
| [GetControlData](./getcontroldata/) | Ottiene i dati del controllo. |
| [GetActiveXControl](./getactivexcontrol/) | Ottiene il controllo ActiveX. |
| [RemoveActiveXControl](./removeactivexcontrol/) | Rimuove il controllo activeX. |
| [GetPaths](./getpaths/) | Ottiene i percorsi di una forma geometrica personalizzata. |
| [GetGeometry](./getgeometry/) | Ottiene la geometria |
| [GetCreateId](./getcreateid/) | Ottiene e imposta l'ID di creazione per questa forma. |
| [SetCreateId](./setcreateid/) | Ottiene e imposta l'ID di creazione per questa forma. |
| [IsDecorative](./isdecorative/) | Indica se l'oggetto è decorativo. |
| [SetIsDecorative](./setisdecorative/) | Indica se l'oggetto è decorativo. |
| [GetActualBox](./getactualbox/) | Ottieni la posizione e le dimensioni effettive della forma (dopo aver applicato rotazione, capovolgimento, ecc.) |
| [FitToTextSize](./fittotextsize/) | Ricalcola un'area di testo adatta a visualizzare tutto il contenuto testuale. |
| [IsSameSetting](./issamesetting/) | Restituisce se la forma è la stessa. |
