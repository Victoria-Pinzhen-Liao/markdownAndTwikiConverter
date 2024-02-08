# Markdown and TWiki Converters

This repository contains two Scala applications designed to convert text between Markdown and TWiki formats. These converters are useful for integrating content across platforms that use different markup languages.

## MarkdownToTwikiConverter

The `MarkdownToTwikiConverter` is a Scala application that converts text from Markdown format to TWiki format. It supports headings, separators, bold and italic text, unordered and ordered lists, code blocks, and hyperlinks.

### Features

- **Headings**: Converts Markdown headings (`#`, `##`, etc.) into TWiki headings (`---+`, `---++`, etc.).
- **Separators**: Converts Markdown horizontal rules (`----`) into TWiki separators (`---`).
- **Text Formatting**: Converts bold (`**bold**`) and italic (`*italic*`) text formatting.
- **Lists**: Converts unordered (`- item`) and ordered (`1. item`) lists.
- **Code Blocks**: Converts Markdown code blocks (`` ``` ``) into TWiki `<verbatim>` blocks.
- **Hyperlinks**: Converts Markdown hyperlinks (`[text](url)`) into TWiki links (`[[url][text]]`).

### Usage

To use the converter, compile and run the Scala application. Ensure your input text is set in the `markdownText` variable.

## TwikiToMarkdownConverter

The `TwikiToMarkdownConverter` is a Scala application that converts text from TWiki format to Markdown format, essentially performing the inverse operation of the MarkdownToTwikiConverter.

### Features

- **Headings**: Converts TWiki headings (`---+`, `---++`, etc.) into Markdown headings (`#`, `##`, etc.).
- **Separators**: Converts TWiki separators (`---`) into Markdown horizontal rules (`----`).
- **Text Formatting**: Converts TWiki bold (`__bold__`) and italic (`_italic_`) text formatting into Markdown.
- **Lists**: Converts TWiki unordered list items (`* item`) into Markdown (`- item`) and assumes a simple conversion for ordered lists.
- **Code Blocks**: Converts TWiki `<verbatim>` blocks into Markdown code blocks (`` ``` ``).
- **Hyperlinks**: Converts TWiki links (`[[url][text]]`) into Markdown hyperlinks (`[text](url)`).

### Usage

Compile and run the Scala application. Ensure your input text is set in the `twikiText` variable.

## Requirements

- Scala
- sbt (Scala Build Tool)
 
