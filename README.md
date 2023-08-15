
🔴**In Analysis Phase**❗🔴
# View Description Language
It is a way to describe views in declarative C# and generate the corresponding views for multiple providers:
* Razor View
* HTML
* Xamarin
* Avalonia
* WPF
* Angular
* Flutter
* .....

# Expected Example
```C#
Page
(
    SingleEntityView<Person>
    (
        Header("Person Details"),
        Field(x => x.Name, "Person Name")
          .Editable()
          .MaxLength(120)
          .Validate(PreBuiltValidation.ArabicName);
    ),
    ButtonsStack(
      Button("Save", PredefinedActions.Save),
      Button("Cancel" ,PredefinedActions.Cancel),
      Button("Delete" ,PredefinedActions.Delete)
  )
)
```
