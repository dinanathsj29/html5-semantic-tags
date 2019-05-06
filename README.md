Section 1. Structuring Content with HTML5 Semantic tags
=====================
1.1. Structure
---------------------
- HTML allows us to structure the document as per the meaning of the content
- Div, Table tags are used to create structure, layout but its not semantic
- HTML Semantic Tags - Structure of the webpage to show meaning, not just layout 
- HTML Semantic Structural/Sectioning Elements helps to create pages more readable, accessible, better search engine results-oriented, easy to modify/update
- A semantic element clearly describes its meaning to both the browser and the developer
> **Note**: HTML5 semantic elements are supported in all modern browsers.

#### HTML Heading Sectioning Elements
h1 to h6
                      
#### HTML5 Semantic Structural/Sectioning Elements

| Tag                 | Use                                                 |
| ----------------- |-----------------------------------------------------|
| `<main>`          | Specifies the main content of a document            |
| `<header>`        | Specifies a header for a document or section        |
| `<nav>`           | Defines navigation links                            |
| `<section>`       | Defines a section in a document                     |
| `<article>`       | Defines an article.                                 |
| `<aside>`         | Defines content aside from the page content         |
| `<footer>`        | Defines a footer for a document or section          |

#### Why HTML5 Semantic Structural/Sectioning Elements introduced?
- Earlier with HTML, developers used/created their own id/class names to style elements like header, footer, top nav, bottom nav, main menu, nav - navigation, main left right top bottom container, content, left article, right sidebar, etc.
- This made it difficult and impossible for search engines to identify the correct web page content also a developer to the browser and edit content
- With the new HTML5 semantic/meaningful elements like (`<header> <footer> <nav> <section> <article> <aside>`), this will become easier
- HTML5 semantic/meaningful elements make pages more readable for machines as well users with accessibility, search engine results, more consistent and easier to use and style
- > According to the W3C, a Semantic Web: "Allows data to be shared and reused across applications, enterprises, and communities"

#### Implementing structural hierarchy
It's really up to you what exactly the elements involved represent, as long as the hierarchy makes sense. You just need to bear in mind a few best practices as you create such structures:
- Preferably you should just `use a single <h1> per page` — this is the top level heading, and all others sit below this in the hierarchy
- Make sure you use the headings in the correct order in the hierarchy. Don't use `<h3>s` to represent subheadings, followed by `<h2>s` to represent sub-subheadings — that doesn't make sense and will lead to weird results

#### Why do we need structure?
- Users looking at a web page tend to scan quickly to find relevant content. If they can't see anything useful within a few seconds, they'll likely get frustrated and go somewhere else.
- Search engines indexing your page consider the contents of headings as important keywords for influencing the page's search rankings. Without headings, your page will perform poorly in terms of `SEO (Search Engine Optimization)`
- Visually impaired people often don't read web pages; they listen to them instead.  If headings are not available, they will be forced to listen to the whole document read out loud

1.2. Outlines
---------------------
- HTML uses Semantic Elements, Headings, Semantic Tags to generate/describe the Document Outline of page content (Document Outline = Topics, Table of Contents, Index)
- Document Outline is used by devices/browsers to scan & search content, navigate to a particular/specific section, also to determine how contents relate to each other
- HTML5 Outliner is used to understand & know the exact outline ie page structure of HTML page/document
- Use outliner utility: https://gsnedders.html1.org/outliner/
- Text Editor like Brackets uses a `Document Outliner Plugin/extension` to show proper document outline/table of contents/topics/Indexing of page
- Brackets -> View menu -> Show Document Outline

1.3. Nav
---------------------
- Represents a section of the document intended for navigation
- The <nav> element defines a set of navigation links
- The HTML <nav> element represents a section of a page whose purpose is to provide navigation links, either within the current document or to other documents
- Common examples of navigation sections are menus, tables of contents, and indexes
> **Note**: It's NOT a rule that all links of a document should be inside an <nav> element The <nav> element is intended only for a major block of navigation links

1.4. Section
---------------------
- Represents a generic document or application section
- The <section> element defines a section in a document
- The HTML <section> element represents a standalone section
- > According to W3C's HTML5 documentation: "A section is a thematic grouping of content, typically with a heading"
- A web page could normally be split into sections for introduction, content, the middle section with left and right sections, etc.

1.5. Article
---------------------
- Represents an independent piece of content of a document, such as a blog entry or newspaper article
- The <article> element specifies independent, self-contained content
- The HTML <article> element represents a self-contained composition in a document
- The HTML <article> tag is used in a blog/forum post, newspaper article, blog entry etc.

1.6. Aside
---------------------
- Represents a piece of content that is only slightly related to the rest of the page
- The <aside> element defines some content aside from the content it is placed in (like a sidebar)
- Asides are frequently presented as sidebars or call-out boxes

1.7. Header
---------------------
- Represents a group of introductory or navigational aids
- The <header> element specifies a header for a document or section
- The <header> element should be used as a container for introductory content
- The HTML <header> element represents introductory content, typically a group of introductory or navigational aids
- It may contain some heading elements but also a logo, a search form, an author name, and other elements
- You may have several <header> elements in one document

1.8. Footer
---------------------
- Represents a footer for a section
- The <footer> element specifies a footer for a document or section
- The HTML <footer> element represents a footer for its nearest sectioning content or sectioning root element
- A footer typically contains information about the author of the section, copyright data or links to related documents
- You may have several <footer> elements in one document

1.9. Div
---------------------
- The div tag is known as `Division, Divider tag`
- The HTML Content Division element (<div>) is the generic container for flow content
- Prior to HTML5 Semantic Tags, the Div tag is used in HTML to make divisions of content in the web page like (text, images, header, footer, navigation bar, etc)
- The <div> tag is an empty container tag, which defines a division or a section by specifying child elements
- With HTML5 Semantic Tags, Div a powerful tag also used for structuring, dividing, Layout, Sectioning page/content with CSS or manipulated with scripts
- The <div> tag is a block-level element, so a line break is placed before and after it
- The Div is the most usable tag in web development because it helps us to separate out data in the web page and we can create a particular section
- It is used to the group of various tags of HTML so that sections can be created and style can be applied to them

1.10. WAI-ARIA
---------------------
- Web Accessibility Initiative-Accessible Rich Internet Application
- It is a set of attributes to help enhance the semantics of a web site or web application to help assistive technologies, such as screen readers for the blind, make sense of certain things that are not native to HTML
- ARIA (WAI-ARIA) is a set of attributes that you can add to HTML elements. These attributes communicate role, state, and property semantics to assistive technologies via the accessibility APIs implemented in browsers
- ARIA (WAI-ARIA) provides the user with a good way to navigate and interact with your site. Make your HTML code as semantic as possible, so that the code is easy to understand for visitors and screen readers
- WAI-ARIA is an incredibly powerful technology that allows developers to easily describe the purpose, state and other functionality of visually rich user interfaces
- **Landmark Roles (Screen Readers and other devices scan and jump to the required role)**
```
    - <header role="banner">
    - <nav role="navigation">
    - <main role="main">
    - <article role="article">
    - <footer role="footer">
    - <aside role="complementary">
    - <footer role="contentinfo">
```

1.11. Websites / Blogs
---------------------
- https://www.w3schools.com/html/html_accessibility.asp
- https://www.w3.org/WAI/standards-guidelines/aria/
- https://www.w3.org/TR/wai-aria/
- https://developer.paciellogroup.com/blog/2013/02/using-wai-aria-landmarks-2013/
