# Crisp-Components

This is a library that provides a collection of UI themes for WPF applications developed using .NET 4.7.2. Designed to provide a modern and crisp look and feel across all controls in your application. The themes are implemented using XAML styles and templates.

## Features
Predefined themes for common UI elements, such as buttons, text boxes, and list boxes.
Easy-to-use XAML styles and templates that can be applied to any WPF control.
Supports light and dark themes.
Fully customizable to fit the needs of your application.
Getting Started
To use the Crisp.Components in your WPF application, follow these steps:

Install the Crisp.Components NuGet package in your project:

```powershell
Install-Package Crisp.Components
```

Add a reference to the Crisp.Components library in your XAML file:

```xml
<Window xmlns:crisp="clr-namespace:Crisp.Components;assembly=Crisp.Components">
```
Apply the desired theme to your window or control using the Style property:

```xaml
<Window Style="{StaticResource BlueTheme}">
  <Grid>
    <!-- Your application content here -->
  </Grid>
</Window>
```

Customize the theme by modifying the predefined styles and templates or defining your own:

```xaml
<Style x:Key="BlueButtonStyle" TargetType="Button">
  <Setter Property="Background" Value="#2196F3" />
  <Setter Property="Foreground" Value="White" />
  <Setter Property="BorderThickness" Value="0" />
  <Setter Property="Padding" Value="8 4" />
  <Setter Property="Template">
    <Setter.Value>
      <ControlTemplate TargetType="Button">
        <Border Background="{TemplateBinding Background}"
                BorderBrush="{TemplateBinding BorderBrush}"
                BorderThickness="{TemplateBinding BorderThickness}"
                Padding="{TemplateBinding Padding}">
          <ContentPresenter HorizontalAlignment="Center"
                            VerticalAlignment="Center" />
        </Border>
      </ControlTemplate>
    </Setter.Value>
  </Setter>
</Style>
```

For more information on using the Crisp.Components, see the official documentation.

## Contributing
Contributions to this library are welcome! If you find a bug or have a feature request, please open an issue on GitHub. If you would like to contribute code, please fork the repository and submit a pull request with your changes.

## License
This library is released under the MIT License. See the LICENSE file for details.
