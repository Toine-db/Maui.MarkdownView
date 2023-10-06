# Maui.MarkdownView
Show Markdown as platform native UI components, so NO HTML output but native controls!

The project goal is a super fast and easy to implement and highly customizable view.
Feel free to add more.

## How to use it

1. Implement a MarkdownView in your XAML that loads Markdown text

optional
1. Customize styling (highly recommended)
2. Customize writer or formatter or handler
3. Customize everything else  

## How it works under the hood

1. CommonMark.NET is used to read Markdown text and turn them into usable c# objects
2. A custom formatter is created to work with the created c# objects (formatter looks like a CommonMark.NET formatter)
3. A custom writer is created to control creation of UI components
4. An UI component generator is created which supplies the UI components (one for every platform)