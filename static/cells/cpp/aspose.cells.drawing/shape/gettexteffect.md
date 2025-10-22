##Aspose::Cells::Drawing::Shape::GetTextEffect method
'Aspose::Cells::Drawing::Shape::GetTextEffect method. Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt in C++.'
## Shape::GetTextEffect method
Returns a [TextEffectFormat](../../texteffectformat/) object that contains text-effect formatting properties for the specified shape. Applies to [Shape](../) objects that represent WordArt.
```cpp
TextEffectFormat Aspose::Cells::Drawing::Shape::GetTextEffect()
```
## Examples
```cpp
if (shape.IsWordArt())
{
TextEffectFormat textEffectFormat = shape.GetTextEffect();
}
```
## See Also
* Class [TextEffectFormat](../../texteffectformat/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
