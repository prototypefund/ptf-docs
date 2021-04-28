---
layout: default
title: Markdown-Begriffsammlung
parent: just-the-docs
nav_order: 99
---

Um eine Sprache zu haben, die einfach lesbar und zugleich schreibbar ist, wurde Markdown entwickelt. So kann der Text in jedem einfachen Texteditor verfasst werden, ohne dass viel Formatierungsanweisungen geschrieben werden müssen.

# Wie schreibe ich Markdown?

Text kann **fett**, _schräg_ oder ~~durchgestrichen~~ werden.

```markdown
Text kann **fett**, _schräg_ oder ~~durchgestrichen~~ werden.
```

[Das ist ein Link zu einer anderen Seite](/index.html).

```markdown
[Das ist ein Link zu einer anderen Seite](/index.html).
```

Zwischen Absätzen wird einfach eine leere Zeile gelassen.

Zwischen Absätzen wird einfach eine leere Zeile gelassen.
Sonst wird der Text einfach weiter geführt.

```markdown
Zwischen Absätzen wird einfach eine leere Zeile gelassen.

Zwischen Absätzen wird einfach eine leere Zeile gelassen.
Sonst wird der Text einfach weiter geführt.
```

# [](#header-1)Überschrift 1. Grades

Das ist ein einfach Absatz nach einer Überschrift (mit Link-Verweis).
Ohne diesen Link kann einen Überschrift auch einfach als
`# Überschrift 1. Grades` am Zeilenanfang geschrieben werden.

```markdown
# [](#header-1)Überschrift 1. Grades

Das ist ein einfach Absatz nach einer Überschrift (mit Link-Verweis).
Ohne diesen Link kann einen Überschrift auch einfach als
`# Überschrift 1. Grades` am Zeilenanfang geschrieben werden.
```

## [](#header-2)Überschrift 2. Grades

> Das ist ein Zitat-Block nnach einer Überschrift.
>
> Die Zeilen verhalten sich ganau so
> wie bei normalen Absätzen.

```markdown
## Überschrift 2. Grades

> Das ist ein Zitat-Block nnach einer Überschrift.
>
> Die Zeilen verhalten sich ganau so
> wie bei normalen Absätzen.
```

### [](#header-3)Überschrift 3. Grades

    Code
    Block

Das ist ein Besispiel eines Code-Blocks mit farblicher Hervorhebung:

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

~~~markdown
### Überschrift 3. Grades

    Code
    Block

Das ist ein Besispiel eines Code-Blocks mit farblicher Hervorhebung:

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```
~~~

#### [](#header-4)Überschrift 4. Grades `mit nicht formatiertem Code-Schnipsel`

* Das ist eine einfache Liste.
- mit drei Punkten
* nach einer Überschrift

```markdown
#### Überschrift 4. Grades `mit nicht formatiertem Code-Schnipsel`

* Das ist eine einfache Liste.
- mit drei Punkten
* nach einer Überschrift
```

##### [](#header-5)Überschrift 5. Grades

1. Das ist eine nummerierte Liste.
    1. Das ist ein Unterpunkt.
    1. Das ist ein noch ein Unterpunkt.
1. Zweiter Punkt nacht der Überschrift
4. Aller guten Dinge sind drei.

```markdown
##### Überschrift 5. Grades

1. Das ist eine nummerierte Liste.
    1. Das ist ein Unterpunkt.
    1. Das ist ein noch ein Unterpunkt.
1. Zweiter Punkt nacht der Überschrift
4. Aller guten Dinge sind drei.
```

###### [](#header-6)Überschrift 6. Grades

| Überschrift 1 | Zweitens           | drei   |
|:--------------|:-------------------|:-------|
| ja            | kommt vor Drittens | gut    |
| nie wieder    | ader vlt. doch     | gut    |
| ja            | ja `aber`          | hmm    |
| ja            | großer Irrtum      | na gut |

```markdown
###### Überschrift 6. Grades

| Überschrift 1 | Zweitens           | drei   |
|:--------------|:-------------------|:-------|
| ja            | kommt vor Drittens | gut    |
| nie wieder    | ader vlt. doch     | gut    |
| ja            | ja `aber`          | hmm    |
| ja            | großer Irrtum      | na gut |
```

### Es gibt horizontale Trenner

* * *

```markdown
* * *
```

### Und Task-Listen

- [ ] Ein TODO
- [ ] Das muss auch noch erlidigt werden.
- [x] Yeah, das ist schon passiert.

```markdown
- [ ] Ein TODO
- [ ] Das muss auch noch erlidigt werden.
- [x] Yeah, das ist schon passiert.
```

### Kleine eingebettet Bilder

In den ersten eckigen Klammern steht der Alt-Text für die HTML-Seite.

![Ein Projekt der Open Knowledge Foundation Deutschland e. V.]({{ site.baseurl }}/assets/images/logo-okfn.svg)

```markdown
![Ein Projekt der Open Knowledge Foundation Deutschland e. V.]({{ site.baseurl }}/assets/images/logo-okfn.svg)
```

### Große, verlinkte Bilder

[![Timeline einer Runde]({{ site.baseurl }}/assets/images/docs/timeline.svg)]({{ site.baseurl }}/assets/images/docs/timeline.svg)

```markdown
[![Timeline einer Runde]({{ site.baseurl }}/assets/images/docs/timeline.svg)]({{ site.baseurl }}/assets/images/docs/timeline.svg)
```

### Für Listen mit Definitionen kann HTML-Code benutzt werden.

<dl>
  <dt>Name</dt>
  <dd>Godzilla</dd>
  <dt>Born</dt>
  <dd>1952</dd>
  <dt>Birthplace</dt>
  <dd>Japan</dd>
  <dt>Color</dt>
  <dd>Green</dd>
</dl>

```html
<dl>
  <dt>Name</dt>
  <dd>Godzilla</dd>
  <dt>Born</dt>
  <dd>1952</dd>
  <dt>Birthplace</dt>
  <dd>Japan</dd>
  <dt>Color</dt>
  <dd>Green</dd>
</dl>
```

#### Mehrere Beschreibungsbegriffe und -werte

Begriff
: Beschreibungswert von "Begriff"

Längerer Begriff
: Längere Beschreibung von "Begriff",
  sie darf auch mehrzeilig sein

Begriff
: Erste Beschreibung von "Begriff",
  sie darf auch mehrzeilig sein

: Zweite Beschreibung von "Begriff",
  sie darf auch mehrzeilig sein

Begriff1
Begriff2
: Eine Beschreibung von "Begriff1" und "Begriff2",
  sie darf auch mehrzeilig sein

Begriff1
Begriff2
: Erste Beschreibung von "Begriff1" und "Begriff2",
  sie darf auch mehrzeilig sein

: Zeite Beschreibung von "Begriff1" und "Begriff2",
  sie darf auch mehrzeilig sein

```markdown
Begriff
: Beschreibungswert von "Begriff"

Längerer Begriff
: Längere Beschreibung von "Begriff",
  sie darf auch mehrzeilig sein

Begriff
: Erste Beschreibung von "Begriff",
  sie darf auch mehrzeilig sein

: Zweite Beschreibung von "Begriff",
  sie darf auch mehrzeilig sein

Begriff1
Begriff2
: Eine Beschreibung von "Begriff1" und "Begriff2",
  sie darf auch mehrzeilig sein

Begriff1
Begriff2
: Erste Beschreibung von "Begriff1" und "Begriff2",
  sie darf auch mehrzeilig sein

: Zeite Beschreibung von "Begriff1" und "Begriff2",
  sie darf auch mehrzeilig sein
```

### Langer Code

```
Lange Einzelzeilen von Source Code sollten nicht gebrochen werden. Sie sollten waagerecht scrollbar sein, wenn sie breiter als der Darstellungsbereich sind.
```

