# Quick Guide to Accessible Design

## Alt-text
Alt text or alternative text are used within HTML code to describe the appearance and functions of an image on a page. Adding an image without proper use of alt tags can be extremely frustrating for individuals navigating your site through assistive technologies. Alternatve text can provide valuable information for low vision or blind screen reader users.
> `<img alt="text alternative">`

[Read more about text alternatives](https://www.abilitynet.org.uk/blog/five-golden-rules-compliant-alt-text "abilitynet.org")

## Keyboard accessible lnks
Some internet users have mobility impairments and can't use a mouse. They rely on keyboard or keyboardlike devices to navigate interactive features of a website. The `Tab` key is used to move forward through elements and `Shift+Tab` to go back.

You should be able to access the following by tabbing:
* links
* menus
* buttons 
* form fields

## Visible focus style
Keyboard users need visual indication of where they are on a page when tabbing. Without a focus style it is difficult to tell where they are.
![Example of a link with focus visible](/focus-visible.png)

```css
:focus {
  outline: 0;
}
```

## color contrast
Visitors with vision impairment may struggle to read text on a low contrast background. WCAG 2.1 Level AA recommends a minimum contrast ration of 4.5:1 for text.

![Color Contrast examples](/contrast.png)

## Semantic html
HTML5 Semantic elements clearly describe meaning to both browsers and the developer.

Examples of non-semantic elements: `<div>` and `<span>` - Tells nothing about its content.

Examples of semantic elements: `<form>`, `<table>`, and `<article>` - Clearly defines its content.

## External links
It is important to warn people using assistive technologies that a new window has opened.
[Waaz Solution](https://waaz.xyz/adding-external-link-indicator-with-css/ "Waaz article about external links")

## Aria Landmark Roles
Aria landmark roles allow developers to identify regions of a page providing immediate benefit. Screen reader users can jump to that section of the page.
The eight ARIA landmark roles are: 
*   role=”banner”
*   role=”navigation” (e.g., a menu)
*   role=”main” (the main content of the page)
*   role=”complementary” (e.g., a sidebar)
*   role=”contentinfo” (meta data about the page, e.g., a copyright statement)
*   role=”search”
*   role=”form”
*   role=”application” (a web application with its own keyboard interface)

## Headings
Headings communicate the organization of the content within a page. Web browsers and assistive technologies can use them to provide in-page navigation. Use html tags with the correct hierarchy without skipping any number.
[Read more about headings](https://www.w3.org/WAI/tutorials/page-structure/headings/ "w3.org")
