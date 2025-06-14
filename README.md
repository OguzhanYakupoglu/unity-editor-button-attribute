# Unity Editor Button Attribute

A lightweight Unity Editor extension that lets you add clickable buttons for methods directly in the Unity Inspector using a simple custom attribute.

## Features

- Add `[Button]` attribute to any method (private, public, or static) without parameters.
- Automatically displays a button in the Inspector with an optional custom label.
- Supports all `MonoBehaviour` scripts.
- Easy to integrate — just add the scripts to your project.

## Usage

1. Add the `Inspector Button Attribute` folder to your project.
2. Decorate any parameterless method in your MonoBehaviour with `[Button]` or `[Button("Custom Label")]`.

```csharp
using UnityEngine;

public class ExampleComponent : MonoBehaviour
{
    [Button]
    private void SayHello()
    {
        Debug.Log("Hello from the inspector button!");
    }

    [Button("Click Me!")]
    public void CustomLabelMethod()
    {
        Debug.Log("Button with a custom label clicked.");
    }
}
