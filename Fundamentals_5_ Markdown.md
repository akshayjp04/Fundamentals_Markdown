# **Fundamentals 5: Markdown**
--------------------
#### **CMDA 3634 Spring 2020**

#### **Due 11:59 PM Eastern, Feb. 19, 11:59 pm**

#### **Collaboration and References**

The work you submit must be your own, but you are allowed to collaborate with your
classmates during class and seek help from teaching staff. You may not copy any code from
a collaborator’s screen, but may discuss concepts and share references. You must list every
classmate you collaborate with in your [references.md](http://references.md/) file.

## **Instructions and Deliverables**
----------------------------
1. You will recreate this document in a markdown file to have the same formang.
2. You will create a [References.md](http://references.md/) file, which must include your full name, collaborators,
and references.
3. You will submit your .md files through Canvas by Feb. 19, 11:59 pm.

## **What is Markdown?** 
---------------------------------
Markdown is a lightweight markup language that you can use to add formang elements to
plaintext text documents. Created by [John Gruber](https://daringfireball.net/projects/markdown/) in 2004, Markdown is now one of the
world’s most popular markup languages.
You can add Markdown formang elements to a plaintext file using a text editor
applicaon. Or you can use one of the many Markdown applicaons for macOS, Windows,
Linux, iOS, and Android operang systems. There are also several web-based applicaons
specifically designed for wring in Markdown.

## **Why Use Markdown?**
-----------------------
You might be wondering why people use Markdown instead of a WYSIWYG editor. Why
write with Markdown when you can press buons in an interface to format your text? As it
turns out, there are a couple different reasons why people use Markdown instead of
WYSIWYG editors.
- Markdown can be used for everything. People use it to create [websites](https://www.markdownguide.org/getting-started/#websites), [documents](https://www.markdownguide.org/getting-started/#documents),
[notes](https://www.markdownguide.org/getting-started/#notes), [books](https://www.markdownguide.org/getting-started/#books), [presentations](https://www.markdownguide.org/getting-started/#presentations), [email messages](https://www.markdownguide.org/getting-started/#email), and [technical documentation](https://www.markdownguide.org/getting-started/#documentation).
- Markdown is portable. Files containing Markdown-formaed text can be opened
using virtually any applicaon.
- Markdown syntax is intuive and, in many cases, it allows for mulple opons, so
writers can choose the formang characters that make the most sense for them.
- Markdown is plaorm independent. You can create Markdown-formaed text on any
device running any operang system.
- Markdown is future proof. Even if the applicaon you’re using stops working at some
point in the future, you’ll sll be able to read your - Markdown-formaed text using a
text eding applicaon.
- Markdown is everywhere. Websites like Reddit and GitHub support Markdown, and
lots of desktop and web-based applicaons support it.

## **How Use Markdown?**
-----------------------------
Markdown doesn’t have all the bells and whistles of word processors like Microso Word,
but it’s good enough for creang basic documents like assignments and leers. You can use
a Markdown document authoring applicaon to create and export Markdown-formaed
documents to PDF or HTML file format. The PDF part is key, because once you have a PDF
document, you can do anything with it — print it, email it, or upload it to a website.
Here are some Markdown document authoring applicaons recommend:
- Mac: [MacDown](https://www.markdownguide.org/tools/macdown), [iA Writer](https://www.markdownguide.org/tools/ia-writer/), or [Marked](https://marked2app.com/)
- iOS / Android: [iA Writer](https://www.markdownguide.org/tools/ia-writer/)
- Windows: [ghostwriter](https://wereturtle.github.io/ghostwriter/) or [Markdown Monster](https://markdownmonster.west-wind.com/)
- Linux: [ReText](https://github.com/retext-project/retext) or [ghostwriter](https://wereturtle.github.io/ghostwriter/)
- Web: [Dillinger](https://www.markdownguide.org/tools/dillinger/) or [StackEdit](https://www.markdownguide.org/tools/stackedit/)

This document was edited in StackEdit, since it integrates some extra features like Latex
and Mermaid.

## **Basic Syntax**
----------------------------

#### **1. Headings**
To create a heading, add number signs ( # ) in front of a word or phrase. The number of
number signs you use should correspond to the heading level (six levels in total).

##### **Example:**
- ## **Title level 2 (```## Title level 2```)**
    -----------------------------------
- ### **Title level 3 (```### Title level 3```)**


- #### **Title level 4 (```#### Title level 4```)**



#### **2. Bold and Italic**
To **bold text**, add two asterisks (``` ** ```) or underscores (``` __ ```) before and aer a word or phrase.
To ***italicize text***, add one asterisk (``` * ```) or underscore (``` _ ```) before and aer a word or phrase.
To emphasize text with **bold and italics** at the same me, add three asterisks (``` *** ```) or
underscores (``` ___ ```) before and aer a word or phrase.

##### **Example:**
- I just love **bold text** (```I just love **bold text**```).
- Italicized text is the _cat’s meow_ (```Italicized text is the _cat’s meow_ ```).
- This text is **really important** (``` This text is **_really important_**```).


#### **3. Block-quotes**
To create a block-quote, add a > in front of a paragraph. For example

```> Some remarks.```
The rendered output looks like this:
>Some remarks.

Block-quotes can contain other Markdown formaed elements. Not all elements can be
used — you’ll need to experiment to see which ones work.
> **The quarterly results look great!**
>- Revenue was off the chart.
> - Profits were higher than ever. 

> Everything is going according to **plan**.


#### **4. Lists**
To create an unordered list, add dashes (``` - ```), asterisks (``` * ```), or plus signs (``` + ```) in front of line
items. Indent one or more items to create a nested list.

##### **Example:**
- First item        
    -  First item a
    -  First item b
- Second item

To create an ordered list, add line items with numbers followed by periods. The numbers
don’t have to be in numerical order, but the list should start with the number one (``` 1. ```).

##### **Example:**
1. First item
    1. First item a
    2. First item b
2. Second Item

Task lists allow you to create a list of items with checkboxes. In Markdown applicaons that
support task lists, checkboxes will be displayed next to the content. To create a task list, add dashes (``` - ```) and brackets with a space (``` [ ] ```) in front of task list items. To select a checkbox,
add an ```x``` in between the brackets (``` [ x ] ```).

##### **Example:**

```- [```x```] Write the press release```
```- [] Update the website```
```- [] Contact the media```

The rendered output looks like this:

[x] Write the press release
    [ ] Update the website
    [ ] Contact the media


#### **Code Blocks**
[Code blocks](https://www.markdownguide.org/basic-syntax/#code-blocks) are normally indented four spaces or one tab. When they’re in a list, indent
them eight spaces or two tabs.

##### Example:  


```
void PrintSquares(){
    for (int i=1;i<10;i++)
        printf("\n i = %d and i*i = %d",i,i*i);
    return;
}
```       

Many Markdown processors support syntax highlighng for fenced code blocks. This
feature allows you to add color highlighng for whatever language your code was wrien
in. To add syntax highlighng, specify a language next to the backcks ( ``` ) before the
fenced code block.

##### **Example:** adding (\```json) and (```) around the previous example produces:


```json
    void PrintSquares(){
        for (int i=1;i<10;i++)
        printf("\n i = %d and i*i = %d",i,i*i);
    return;
    } 
```

adding (\```python) and (```) produces:
```python
n = int(input('Type a number, then its factorial     will be printed: '))
if n < 0:
    raise ValueError('You must enter a positive number')
fact = 1
i   = 2
while i <= n:
    fact = fact * i
    i += 1
print(fact)
```

#### **6. Links**

To create a link, enclose the link text or tle in brackets (e.g., [```Markdown Guide```] ) and then
follow it immediately with the URL in parentheses (e.g.,
```(https://www.markdownguide.org/) ```).
```Extra information at [Markdown Guide](https://www.markdownguide.org/).```
The rendered output looks like this:
Extra information at [Markdown Guide](https://www.markdownguide.org/).
To **emphasize links**, add asterisks before and after the brackets and parentheses.

#### **7. URLs and Email Addresses**
To quickly turn a URL or email address into a link, enclose it in angle brackets.
```<https://vt.edu>```
```<some_id@vt.edu>```
The rendered output looks like this:
<https://vt.edu>
<some_id@vt.edu>

#### **8. Images**
To add an image, add an exclamaon mark ( ! ), followed by alt text in brackets, and the
path or URL to the image asset in parentheses. You can oponally add a tle aer the URL
in the parentheses.
```![VT image](https://image_adress)```
For example, we can include the image located at the following address.
```https://1000logos.net/wp-content/uploads/2018/08/Virginia-Tech-Emblem.jpg```
![VT image](https://1000logos.net/wp-content/uploads/2018/08/Virginia-Tech-Emblem.jpg)

> How to get an image’s address or URL:
> 1. Go the webpage the image is on.
> 2. Make sure you click on the image to ensure it is no link.
> 3. For PC’s, right-click, and for Macs, hold down the control (Ctrl) and click  on the
image itself.
> 4. A menu of opons should appear. In Google Chrome, select “Copy Image
Address”

### **Additional Resources**
---------------------
There are lots of resources you can use to learn Markdown. Here are some other
introductory resources:
- [John Gruber’s Markdown documentaon](https://daringfireball.net/projects/markdown/). The original guide wrien by the creator of
Markdown.
- [Markdown Tutorial](https://www.markdowntutorial.com/). An open source website that allows you to try Markdown in your
web browser. It includes: [cheat-sheet](https://www.markdownguide.org/cheat-sheet/), [basic syntax](https://www.markdownguide.org/basic-syntax/), and [extended syntax](https://www.markdownguide.org/extended-syntax/).
- [Awesome Markdown](https://github.com/mundimark/awesome-markdown). A list of Markdown tools and learning resources.
- [Typeseng Markdown](https://dave.autonoma.ca/blog/2019/05/22/typesetting-markdown-part-1). A mul-part series that describes an ecosystem for
typeseng Markdown documents using [pandoc](https://pandoc.org/) and [ConTeXt](https://www.contextgarden.net/).
- [Markdown Guide](https://www.markdownguide.org/). A free and open-source reference guide that explains how to use
Markdown, the simple and easy-to-use markup language you can use to format
virtually any document
