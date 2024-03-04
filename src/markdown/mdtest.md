${toc}

---
__Advertisement :)__

- __[pica](https://nodeca.github.io/pica/demo/)__ - high quality and fast image
  resize in browser.
- __[babelfish](https://github.com/nodeca/babelfish/)__ - developer friendly
  i18n with plurals support and easy syntax.

You will like those projects!
---

# h1 Heading 8-)
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading

## Horizontal Rules

Underscore
___

Dash
---

Star
***

+++ <visible_text>
<hidden_text>
+++

## Video
@[youtube](KuSCpxg8KT8)


## Typographic replacements

Enable typographer option to see result.

(c) (C) (r) (R) (tm) (TM) (p) (P) +-

test.. test... test..... test?..... test!....

!!!!!! ???? ,,  -- ---

"Smartypants, double quotes" and 'single quotes'


## Emphasis

**This is bold text**

__This is bold text__

*This is italic text*

_This is italic text_

~~Strikethrough~~


## Blockquotes


> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.


## Lists

Unordered

+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!

Ordered

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa


1. You can use sequential numbers...
1. ...or keep all the numbers as `1.`

Start numbering with offset:

57. foo
1. bar


## Code

Inline `code`

Indented code

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code


Block code "fences"

```
Sample text here...
```

Syntax highlighting js

```js
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
```

Syntax highlighting python

```python
class Someclass:
  x: Object
  y: Object
```


## Tables

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Right aligned columns

| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |


## Links

[local link text](/auth/login)

[anchor link](#images)

[external link text](http://dev.nodeca.com)

[link with title](http://nodeca.github.io/pica/demo/ "title text!")

Autoconverted link https://github.com/nodeca/pica (enable linkify to see)


## Images

![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

Like links, Images also have a footnote style syntax

![Alt text][id]

With a reference later in the document defining the URL location:

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"


## Plugins

The killer feature of `markdown-it` is very effective support of
[syntax plugins](https://www.npmjs.org/browse/keyword/markdown-it-plugin).


### [Emojies](https://github.com/markdown-it/markdown-it-emoji)

> Classic markup: :wink: :cry: :laughing: :yum:
>
> Shortcuts (emoticons): :-) :-( 8-) ;)

see [how to change output](https://github.com/markdown-it/markdown-it-emoji#change-output) with twemoji.


### [Subscript](https://github.com/markdown-it/markdown-it-sub) / [Superscript](https://github.com/markdown-it/markdown-it-sup)

- 19^th^
- H~2~O


### [\<ins>](https://github.com/markdown-it/markdown-it-ins)

++Inserted text++


### [\<mark>](https://github.com/markdown-it/markdown-it-mark)

==Marked text==


### [Footnotes](https://github.com/markdown-it/markdown-it-footnote)

Footnote 1 link[^first].

Footnote 2 link[^second].

Inline footnote^[Text of inline footnote] definition.

Duplicated footnote reference[^second].

[^first]: Footnote **can have markup**

    and multiple paragraphs.

[^second]: Footnote text.


### [Definition lists](https://github.com/markdown-it/markdown-it-deflist)

Term 1

:   Definition 1
with lazy continuation.

Term 2 with *inline markup*

:   Definition 2

        { some code, part of Definition 2 }

    Third paragraph of definition 2.

_Compact style:_

Term 1
~ Definition 1

Term 2
~ Definition 2a
~ Definition 2b


### [Abbreviations](https://github.com/markdown-it/markdown-it-abbr)

This is HTML abbreviation example.

It converts "HTML", but keep intact partial entries like "xxxHTMLyyy" and so on.

*[HTML]: Hyper Text Markup Language

### [Custom containers](https://github.com/markdown-it/markdown-it-container)

::: warning
*here be dragons*
:::


## Linkify content
%
% Regular links
%
My http://example.com site
My http://example.com/ site
http://example.com/foo_bar/
http://user:pass@example.com:8080
http://user@example.com
http://user@example.com:8080
http://user:pass@example.com
[https](https://www.ibm.com)[mailto](mailto:someone@ibm.com) % should not catch as auth (before @ in big link)
http://example.com:8080
http://example.com/?foo=bar
http://example.com?foo=bar
http://example.com/#foo=bar
http://example.com#foo=bar
http://a.in
HTTP://GOOGLE.COM
http://example.invalid % don't restrict root domain when schema exists
http://inrgess2 % Allow local domains to end with digit
http://999      % ..and start with digit, and have digits only
http://host-name % local domain with dash
>>example.com % markdown blockquote
>>http://example.com % markdown blockquote
http://lyricstranslate.com/en/someone-you-നിന്നെ-പോലൊരാള്‍.html % With control character

%
% localhost (only with protocol allowed)
%
//localhost
//test.123
http://localhost:8000?

%
% Other protocols
%
My ssl https://example.com site
My ftp://example.com site

%
% Neutral proto
%
My ssl //example.com site

%
% IPs
%
4.4.4.4
192.168.1.1/abc

%
% Fuzzy
%
test.example@http://vk.com
text:http://example.com/
google.com
google.com: // no port
s.l.o.w.io
a-b.com
GOOGLE.COM.
google.xxx // known tld

%
% Correct termination for . , ! ? [] {} () "" ''
%
(Scoped http://example.com/foo_bar)
http://example.com/foo_bar_(wiki)
http://foo.com/blah_blah_[other]
http://foo.com/blah_blah_{I'm_king}
http://foo.com/blah_blah_I'm_king
http://www.kmart.com/bestway-10'-x-30inch-steel-pro-frame-pool/p-004W007538417001P
http://foo.com/blah_blah_"doublequoted"
http://foo.com/blah_blah_'singlequoted'
(Scoped like http://example.com/foo_bar)
[Scoped like http://example.com/foo_bar]
{Scoped like http://example.com/foo_bar}
"Quoted like http://example.com/foo_bar"
'Quoted like http://example.com/foo_bar'
[example.com/foo_bar.jpg)]
http://example.com/foo_bar.jpg.
http://example.com/foo_bar/.
http://example.com/foo_bar,
http://index-of.es/Android/Professional.Android.2.Application.Development.(Wrox,.2010,.0470565527).pdf
https://github.com/markdown-it/linkify-it/compare/360b13a733f521a8d4903d3a5e1e46c357e9d3ce...f580766349525150a80a32987bb47c2d592efc33
https://www.google.com/search?sxsrf=ACYBGNTJFmX-GjNJ8fM-2LCkqyNyxGU1Ng%3A1575534146332&ei=Qr7oXf7rE4rRrgSEgrmoAw&q=clover&oq=clover&gs_l=psy-ab.3..0i67j0l9.2986.3947..4187...0.2..0.281.1366.1j0j5......0....1..gws-wiz.......0i71j35i39j0i131.qWp1nz4IJVA&ved=0ahUKEwj-lP6Iip7mAhWKqIsKHQRBDjUQ4dUDCAs&uact=5
https://ourworldindata.org/grapher/covid-deaths-days-since-per-million?zoomToSelection=true&time=9..&country=FRA+DEU+ITA+ESP+GBR+USA+CAN
http://example.com/foo_bar...
http://172.26.142.48/viewerjs/#../0529/slides.pdf
http://example.com/foo_bar..
http://example.com/foo_bar?p=10.
https://www.google.ru/maps/@59.9393895,30.3165389,15z?hl=ru
https://www.google.com/maps/place/New+York,+NY,+USA/@40.702271,-73.9968471,11z/data=!4m2!3m1!1s0x89c24fa5d33f083b:0xc80b8f06e177fe62?hl=en
https://www.google.com/analytics/web/?hl=ru&pli=1#report/visitors-overview/a26895874w20458057p96934174/
http://business.timesonline.co.uk/article/0,,9065-2473189,00.html
https://google.com/mail/u/0/#label/!!!Today/15c9b8193da01e65
http://example.com/123!
http://example.com/123!!!
http://example.com/foo--bar
See http://example.com/123; Example link.
http://example.com/123;123

% some sites have links with trailing dashes
http://www.bloomberg.com/news/articles/2015-06-26/from-deutsche-bank-to-siemens-what-s-troubling-germany-inc-
http://example.com/foo-with-trailing-dash-dot-.
<http://domain.com>
<http://domain.com>.
<http://domain.com/foo>
<http://domain.com/foo>.
<domain.com>
<domain.com>.
<domain.com/foo>
<user@domain.com>
<user@domain.com>.
<mailto:user@domain.com>

%
% Emails
%
test."foo".bar@gmail.co.uk!
"test@example.com"
name@example.com
>>name@example.com % markdown blockquote
mailto:name@example.com
MAILTO:NAME@EXAMPLE.COM
mailto:foo_bar@example.com
foo+bar@gmail.com
192.168.1.1@gmail.com
mailto:foo@bar      % explicit protocol make it valid
(foobar email@example.com)
(email@example.com foobar)
(email@example.com)

%
% International
%
http://✪df.ws/123
http://xn--df-oiy.ws/123
a.ws
➡.ws/䨹
example.com/䨹
президент.рф

% Links below provided by diaspora* guys, to make sure regressions will not happen.
% Those left here for historic reasons.
http://www.bürgerentscheid-krankenhäuser.de
http://www.xn--brgerentscheid-krankenhuser-xkc78d.de
http://bündnis-für-krankenhäuser.de/wp-content/uploads/2011/11/cropped-logohp.jpg
http://xn--bndnis-fr-krankenhuser-i5b27cha.de/wp-content/uploads/2011/11/cropped-logohp.jpg
http://ﻡﻮﻘﻋ.ﻭﺯﺍﺭﺓ-ﺍﻼﺘﺻﺍﻼﺗ.ﻢﺻﺭ/
http://xn--4gbrim.xn----ymcbaaajlc6dj7bxne2c.xn--wgbh1c/

%
% Others...
%
｜www.google.com/www.google.com/foo｜bar    % #46, asian vertical pipes
｜test@google.com｜bar
｜http://google.com｜bar

%
% Domains with multiple dashes
%
https://5b0ee223b312746c1659db3f--thelounge-chat.netlify.com/docs/
www.a--b.com
www.c--u.com
http://a---b.com/


%
% Not links
%
example.invalid
example.invalid/
http://.example.com
http://-example.com
hppt://example.com
example.coma
-example.coma
foo.123
localhost           % only with protocol allowed
localhost/
///localhost        % 3 '/' not allowed
///test.com
//test              % Don't allow single level protocol-less domains to avoid false positives

_http://example.com
_//example.com
_example.com
http://example.com_
@example.com

node.js and io.js

http://
http://.
http://..
http://#
http://##
http://?
http://??
google.com:500000 // invalid port
show image.jpg
path:to:file.pm
/path/to/file.pl

%
% Not IPv4
%
1.2.3.4.5
1.2.3
1.2.3.400
1000.2.3.4
a1.2.3.4
1.2.3.4a

%
% Not email
%
foo@bar     % Should be at second level domain & with correct tld
mailto:bar
