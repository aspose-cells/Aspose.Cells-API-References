---
title: TextBoxActiveXControl
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет элемент управления ActiveX текстового поля.
type: docs
weight: 1720
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/
---
## TextBoxActiveXControl class

Представляет элемент управления ActiveX текстового поля.

```csharp
public class TextBoxActiveXControl : ActiveXControl
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor) { get; set; } | Получает и устанавливает цвет фона ole. |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor) { get; set; } | Получает и устанавливает цвет фона ole. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle) { get; set; } | Получает и устанавливает тип границы, используемой элементом управления. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data) { get; } | Получает и устанавливает двоичные данные элемента управления. |
| [DropButtonStyle](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle) { get; set; } | Указывает символ, отображаемый на раскрывающейся кнопке |
| [EnterFieldBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior) { get; set; } | Определяет поведение выбора при входе в элемент управления. True указывает, что выбор остается неизменным с момента последней активности элемента управления. False указывает, что весь текст в элементе управления будет выделен при входе в элемент управления. |
| [EnterKeyBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior) { get; set; } | Определяет поведение клавиши ENTER. True указывает, что нажатие ENTER создаст новую строку. False указывает, что нажатие ENTER переместит фокус на следующий объект в порядке табуляции. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font) { get; } | Представляет шрифт элемента управления. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor) { get; set; } | Получает и задает ole цвет переднего плана. |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height) { get; set; } | Получает и задает высоту элемента управления в пунктах. |
| [HideSelection](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection) { get; set; } | Указывает, отображается ли выделенный текст в элементе управления, когда элемент управления не имеет фокуса. |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode) { get; set; } | Получает и задает режим времени выполнения по умолчанию редактора метода ввода для элемента управления, когда он получает фокус. |
| [IntegralHeight](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight) { get; set; } | Указывает, будет ли элемент управления отображать только полные строки текста без отображения каких-либо частичных строк. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize) { get; set; } | Указывает, будет ли автоматически изменяться размер элемента управления для отображения всего его содержимого. |
| [IsAutoTab](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab) { get; set; } | Указывает, будет ли фокус автоматически перемещаться к следующему элементу управления, когда пользователь вводит максимальное количество символов. |
| virtual [IsAutoWordSelected](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected) { get; set; } | Определяет базовую единицу, используемую для расширения выделения. True указывает, что основной единицей является один символ. false указывает, что основной единицей является целое слово. |
| [IsDragBehaviorEnabled](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled) { get; set; } | Указывает, разрешено ли перетаскивание для элемента управления. |
| [IsEditable](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable) { get; set; } | Указывает, может ли пользователь вводить текст в элемент управления. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled) { get; set; } | Указывает, может ли элемент управления получать фокус и реагировать на события, созданные пользователем. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked) { get; set; } | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [IsMultiLine](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline) { get; set; } | Указывает, может ли элемент управления отображать более одной строки текста. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent) { get; set; } | Указывает, является ли элемент управления прозрачным. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible) { get; set; } | Указывает, виден ли этот элемент управления. |
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped) { get; set; } | Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell) { get; set; } | Получает и устанавливает связанную ячейку. |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange) { get; set; } | Получает и задает диапазон заполнения списка. |
| [MaxLength](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength) { get; set; } | Получает и устанавливает максимальное количество символов |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon) { get; set; } | Получает и задает пользовательский значок для отображения в качестве указателя мыши для элемента управления. |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer) { get; set; } | Получает и задает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [PasswordChar](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar) { get; set; } | Получает и задает символ, который будет отображаться вместо введенных символов. |
| [ScrollBars](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars) { get; set; } | Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, и то, и другое или ни одно из них. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow) { get; set; } | Указывает, показывать ли тень. |
| [ShowDropButtonTypeWhen](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen) { get; set; } | Указывает символ, отображаемый на раскрывающейся кнопке |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect) { get; set; } | Получает и задает специальный эффект элемента управления. |
| [TabKeyBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior) { get; set; } | Указывает, разрешены ли символы табуляции в тексте элемента управления. |
| [Text](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text) { get; set; } | Получает и устанавливает текст элемента управления. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign) { get; set; } | Представляет способ выравнивания текста, используемого элементом управления. |
| override [Type](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/type) { get; } | Получает тип элемента управления ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width) { get; set; } | Получает и задает ширину элемента управления в пунктах. |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook) { get; } | Получает[`Workbook`](../activexcontrolbase/workbook) объект. |

### Смотрите также

* class [ActiveXControl](../activexcontrol)
* пространство имен [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
