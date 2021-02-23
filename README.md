# <center>Mastering Markdown</center>

![markdown](images/markdown.jpg)

Markdown is a plain text formatting syntax for writers. It allows you to quickly write structured content for the web, and have it seamlessly converted to clean, structured HTML.

Once you get the hang of Markdown, it’s an incredibly powerful writing tool which will allow you to write rich content for the web far faster than almost any other method.

Here’s a quick example of Markdown in action:

    The *quick* brown fox, jumped **over** the lazy [dog](https://en.wikipedia.org/wiki/Dog).

becomes

The *quick* brown fox, jumped **over** the lazy [dog](https://en.wikipedia.org/wiki/Dog).


## :baby: Basic Markdown

### Paragraphs

    This is paragraph 1.
    No empty line in between, so I am still on paragraph 1.

    This seems like paragraph 2.

    Shouldn't this be paragraph 3 then.

A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines. If two lines need to be converted into paragraphs, you must leave an empty space between them.

### Headings

    # Heading 1
    ## Heading 2
    ### Heading 3

Headings in Markdown are any line which is prefixed with a # symbol. The number of hashes indicates the level of the heading. One hash is converted to an *h1*, two hashes to an *h2* and so on. There are a total of 6 levels which you can make use of - but for most writing, you’ll rarely ever need more than 3.

### Lists

    * Milk
    * Bread
        * Wholegrain
    * Butter

</blankline>

    1. Tidy the kitchen
    2. Prepare ingredients
    3. Cook delicious things

Lists are a formatting nightmare in HTML, but Markdown lists are incredibly easy to manage. For a bullet list, just prefix each like with a `*`, `-` or `+` and they will be converted to dots. You can also create nested lists; just indent a line with 4 spaces and it will be nested under the line above.

For numbered lists, do exactly the same thing - but use numbers!

### Quotes

    > To be or not to be, that is the question.

When you want to add a quote in Markdown, it’s exactly the same as the formatting which you may already be familiar with from your email app of choice when you reply to someone.

### Text

    *italic*
    **bold**
    ***bold-italic***
    ~~strikethrough~~
    [link](https://example.com)

If you want to emphasise a word a *little* bit, wrap it in asterisks. For something that needs **more** emphasis: double asterisks. If you really want to ***drive*** the point home, use triple asterisks. If you prefer, you can also use underscores - they’re completely interchangeable.

To add a link: wrap the text which you want to be linked in square brackets, followed by the URL to be linked to in parenthesis.

### Images

    ![description](https://website.com/image.jpg)

Markdown images have exactly the same formatting as a link, except they’re prefixed with a `!`. This time, the text in brackets is the descriptive text for the image.

![woo-hoo](images/woo-hoo.jpg)


## :nerd_face: Advanced Markdown

### Escaping

    \*literally\*

What if you literally want to type *literally* - without it appearing in italics? Escaping Markdown characters with a back-slash \ allows you to use any characters which might be getting accidentally converted into HTML.

### Reference Lists & Titles

    The quick brown [fox][1], jumped over the lazy [dog][2].

    [1]: https://en.wikipedia.org/wiki/Fox "Wikipedia: Fox"
    [2]: https://en.wikipedia.org/wiki/Dog "Wikipedia: Dog"

If you prefer to use reference lists for your attribution, Markdown can handle this, too. In the above example, all of the links are kept separate in Markdown (so it's easy to read even in its raw format), and then inserted directly as normal links when converted to HTML.

### Tables

You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe `|`:

    Cat Breeds | Temperament
    --- | ---
    Maine Coon | Gentle giant
    Siamese | Chatty Cathy
    Panther | Less gentle giant

becomes

Cat Breeds | Temperament
--- | ---
Maine Coon | Gentle giant
Siamese | Chatty Cathy
Panther | Less gentle giant

### Embedding HTML

    <button class="button-save large">Big Fat Button</button>

Possibly the coolest feature of Markdown is that it also just supports plain old HTML. If you find yourself stuck and unable to do what you want in Markdown - you can simply write in regular HTML and it will work just fine.

### Code Snippets

    Some text with an inline `code` snippet

If you’re a technical writer, you may want to use example snippets of code to teach your readers a particular syntax (like I’m doing, with this very blog post). Using a single back-tick around a word in a sentence, you can show a quick `code` snippet.

### Syntax Highlighting

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

Many Markdown processors support syntax highlighting for fenced code blocks. This feature allows you to add color highlighting for whatever language your code was written in. To add syntax highlighting, specify a language next to the backticks before the three backticks.

### Emoji

Some Markdown applications allow you to insert emoji by typing emoji shortcodes. These begin and end with a colon and include the name of an emoji.

    Gone camping! :tent: Be back soon.  
    That is so funny! :joy:

becomes

Gone camping! :tent: Be back soon.  
That is so funny! :joy:

Here's a [list of emoji shortcodes](https://gist.github.com/rxaviers/7360908) to use!
