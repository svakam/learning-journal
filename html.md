# Duckett Notes: Intro to Structuring Web Pages with HTML
10/15/2019
## Chapter 18: Process and Design
 This chapter discusses a process to use when creating a website. The process centers the website design around _user experience_; that is,understanding the site's audience, organizing information in a friendly way, presenting information to achieve the user's goals, and tips to make websites more attractive to users. 
- How to approach building a site
- Understanding your audience and their needs
- How to present information visitors want to see

#### Who is the site for?
- Every site should be made for the _target audience_. Accomplishing this involves understanding _who_ the audience is. 
- Ask yourself/your client questions about the target audience. 
    
  - Target audience: Indivdiuals
    - Age range?
    - Women vs. men?
    - Country of residence?
    - Urban vs. rural?
    - Occupation? 
    - Education level?
  - Target audience: Companies
    - Size of company/dept?
    - Position of people in company?
    - Budget?

  - _"What would x individual or y company want in this situation?"_

#### Why people visit the website
- Now that it's known who the visitors are, consider _why_ they're visiting. 
- Design the content around the _goals_ and _motivations_ of the users. 
  - Key motivations
    - Looking for entertainment, or achieving a specific goal?
    - If specific goal, is it personal vs. professional?
    - Is spending time on this website essential vs. on a luxury basis?
  - Specific goals
    - Do they want general info, or are they after specifics?
    - Are they already familiar with the service/product, or do they need an introduction?
    - Are they looking for time-sensitive info (e.g. latest news)?
    - Do they want to discover new information about a product/service to make a decision on purchasing? 
    - Is it necessary to contact you?
- Make a list of reasons why people would want to visit the site. Go so far as to assign random names and random scenarios to each name, and how it connects to their goals/motivations and the website. 
  - _Malia's computer mouse broke after mere hours of use, and wants to file a complaint on the brand's website via its contact info._

#### How often people will visit the site
- Sites need to be updated based on it's about. For example, a fashion website will need to be updated far more than an evidence-based informational page. 
  - Goods/services
    - How often are purchases made?
    - How often is service changed?
  - Information
    - How often is the subject updated?
    - Is the information updated often, or just once? How often does the user want/need it?
- Scheduling updates > ad hoc updates. 
- Sections of a website would be updated more than others. 

#### Site maps
- Once you know what the audience is, why they're visiting, and how often they'll visit, make a map of the various page names and how they'll link to each other. 

#### Wireframes
- This is a sketch of the key _information_ that needs to go on each page of the site. In other words, it is a _visual representation_ of how each page looks, with notes of where information goes and what the information's purpose is to the user. 
  - Ex. header: big logo up top; nav bar of links to home/products/services/about/contact. main: product photography, key selling points, buy button bottom right. footer: company news, testimonials, sales offers; copyright

#### Getting message across using design
- The primary aim of any visual design is __communication__. 
- Content: logos, links, login, ability to comment
- Prioritizing: making aspects of the page look distinct from another (images, font size, color, style for example)
- Organizing: putting information into blocks or chunks allows your user to recognize friendly real-world patterns

----------------

## Chapter 1: Structure
#### This chapter introduces the concept of HTML structuring a web page, and HTML tags/elements and adding them to the document. 

#### Structure on pages is used in our everyday lives. 
- Newspapers, iPad articles, and the like use headlines, text, images, and subheadings to let the user travel easily around the page and disseminate information well. 

#### Word documents have structure as well. 
- Paragraphs, headings, etc. 

#### What is HTML?
- HTML is Hyper-Text Markup Language. 
- **Elements:** HTML code are characters living inside _angled brackets_. 
- **Tags:** Elements are made of two tags: an _opening tag_ and a _closing tag_. Tags can be _self-closing_ as well (e.g. images). 

#### HTML uses elements to desribe the structure of pages. 
- Tags act like containers, which tell us what lives inside them and what it's about. 

#### Tags:
- Left-angle bracket, character, right-angle bracket
  - `<p>`
  - `</p>`

#### Attributes tell us more about elements. 
- They appear in the opening tag of the element and are made of a _name_ and a _value_, separated by an _equals_ sign. 
  - `<p lang=en-us>English paragraph</p>`

#### Body, head, title:
- `<body></body>`
  - Everything inside this element is shown in the main browser window. 
- `<head></head>`
  - This element contains information _about_ the page. 
- `<title></title>`
  - This is usually found inside `<head>`. Its contents are shown at the top of the browser or on the tab of the page. 

#### _Look at other web pages to learn by example._
- View the source via browser tools. 
-----------

## Chapter 17: HTML5 Layout

#### Traditional HTML layouts
- `<div>`
  - These elements were very commonly used to group together related elements on the page (e.g. elements that form header vs. article vs. footer). `class` or `id` attributes were used for the opening tag of this element to indicate the role of the given `<div>` on the page. 
    - `<div id="header">` `<div id="nav">`
    - `<div id="content">` `<div id="article">` `<div class="article">` `<div class="article">`
    - `<div id="footer">`

#### HTML5 layouts
- New set of elements allow the division of page and content of the code easier to follow. 
- Many `<div>` elements have been replaced by new HTML5 layout elements. 
  - Instead of `<div id="footer">`, just `<footer>`
  - Instead of `<div id="sidebar">`, just `<aside>`

#### More on `<header>` and `<footer>`
- `<header>` and `<footer>` for the top and bottom, respectively, of every page
- Also used to denote headers or footers within an `<article>`, for instance

#### Navigation `<nav>`
- Used to contain _major navigational blocks_ on the site. 
- Tend to be associated with lists of links to other major pages. 

#### Articles `<article>`
- Contains any section of a page that could stand alone. 
- Could be an individual article, blog entry, comment/forum post, or any _independent piece of content_. 
- They can be nested inside each other for 'sub-articles' to make "child" articles. 

#### Asides `<aside>`
- If used within an `<article>`, it is used for non-essential but related information to the `<article>`'s content. 
- If used outside of an `<article>`, it is literally an 'aside' to the whole page and, for instance, can be used as links to other areas of the site unrelated or related to the current page.

#### Sections `<section>`
- Groups related content together, and each section would have its own `<heading>`. 
- On a homepage, there may be several of these that contain differing information. 
- Within `<section>`'s, multiple `<articles>` may be abound that are related and have a theme/purpose. 
- Should not be used as a wrapper; leave this to `<div>` (?). 

#### Heading groups `<hgroup>`
- Tricky to understand, but easier when visualized; it is used to group together a set of 1+ `<h1>` through `<h6>` elements so they are treated as one heading. 
- An `<h3>` heading can be treated a subtitle to an `<h2>` heading, which would together be opened and closed by `<hgroup></hgroup>`. 
- Apparently its use is controversial? 

#### Figures `<figure>` `<figcaption>`
- `<figure>` contains any _content that is referenced from the main flow of an article_. The article should still make sense if the content of `<figure>` was moved. If the information contained within `<figure>` is essential to the article, it should not be treated as a figure (figures should be used only as reference, and is not important for the flow of information of a page). 
- `<figcaption>` is a caption of the figure. 
- Can be used for more than images (videos, graphs, diagrams, etc.). 

#### Sectioning elements `<div>`
- Although HTML5 steered away from the use of this, it is still an important element for when there is _no other element_ that can describe the information of code at hand (thus, it can be ascertained that the newer HTML5 elements should be used only when appropriate). 

#### Linking around block-level elements
- `<a>` is used around a _block-level element_ that contains _child elements_. This allows the entire block to become a link. 
- `<a href="introduction.html>` `<article>` `...` `</article>``</a>`

-----------

## Chapter 8: Extra Markup

This chapter has to do with the evolution of HTML, adding code comments, global attributes (class vs. id), grouping together elements when no other is suitable, embedding page within a page (iframes), adding info about web page using `<meta>`, and adding other characters. 

#### Evolution of HTML
- HTML4 (1997), XHTML 1.0 (2000), HTML5 (current). 

#### Doctypes
- Due to several versions of HTML existing, `DOCTYPE` declaration tells the browser which HTML is being used. 
- HTML5: `<!DOCTYPE html>`
- HTML4: `<!DOCTYPE html PUBLIC>`
- (check out page 181 for other versions)

#### Comments in HTML
- `<!-- comment goes here -->`
- Comment not be visible in user's browser. 

#### ID attribute
- Every HTML element can carry the `id` attribute. This is important later for CSS, when you want to style only 1 particular element based on the `id` it has. This is additionally important for JS, when the `id` attribute is referenced to work only with that element. `id` is a _global attribute_ because it can be _used on any element._
- `<p id="pullquote"> content </p>`

#### Class attribute
- Every element can also carry a `class` attribute. 
- This is important when you want to identify _several_ elements as being different from other elements, as opposed to just 1 element being unique from otehrs. 
- Once again, `class` can be referenced via CSS or JS to modify the content within the element. 
- `<p class="important"> content </p>`
- `<p class="important> content2 </p>`

#### Block elements
- Some elements will appear to start on a new line in the browser window. 
- `<h1>`, `<p>`, `<ul>`, `<li>` are examples that cause block elements. 
- For example, this very block right here! Except this is in markdown. 

#### Inline elements
- Some elements will appear to continue in the same line as neighboring elements. 
- `<a>`, `<b>`, `<em>`, `<img>`. 
- For example, `hi <b> hello </b>` -> hi <b>hello</b>. 

#### Grouping text and elements in a block
- Here we go again: `<div>`. 
- It allows grouping elements together in one block-level box. 
- In a browser, `<div>` content starts a new line. 
- Using `id` or `class` on `<div>` is important for CSS/JS. 
- Add comments! 

#### Grouping text and elements inline
- `<span>` is the _inline equivalent_ of `<div>`. 
- Used to:
  - Contain a section of text when no other element can be used to differentiate it 
  - Contain other inline elements
  - Subsequently control the "inline" text via CSS; thus, `id` and `class` can be used. 

#### iframes
- `<iframe>` is abbreviated from "inline frame"; it's used to create a window on the page, often used for Google Maps. 
- Attributes include `width=<number>`, `height=<number>`, `src=""`, `scrolling="yes"` (or no), and `seamless`. 

#### Information about your pages
- You'll want to make sure your webpage can be referenced; for example, searchable on Google. 
- `<meta>` lives inside `<head>` and conatins information about the web page. It is not visible on the user's browser, but the opening tag contains attributes such as `meta name="description" content=""`, `"robots"`, and `"keywords"`. Others include author, prgama, and expires. 

