---
title: Markdown-Syntax - Listen
description: Markdown-Syntax - Listen
---

## Listen

*Markdown* unterstützt Sie bei der Erstellung von unsortierten und sortierten/ nummerierten Listen. Für die Unterscheidung werden jeweils nur andere Eintragskennzeichen verwendet. Das Eintragskennzeichen muss aber immer nach rechts hin mit mindestens einem Leerzeichen oder einem Tab vom Eintragstext abgegrenzt werden. Normalerweise stehen Listen immer am linken Rand. Sie können jedoch bis zu drei Leerzeichen eingerückt werden.

### Unsortierte Listen

Bei unsortierten Listen kann als Eintragskennzeichen das Sternchen, das Plus oder der Bindestrich verwendet werden. Innerhalb einer Liste *können* die Eintragskennzeichen auch gemischt werden. Der Übersichtlichkeit halber sollte man dies aber nicht machen.

Die folgenden *Markdown*-Beispiele sind also, was den daraus erzeugten HTML-Quelltext angeht, identisch.

{% highlight text %}
* Eintrag 1
* Eintrag 2
* Eintrag 3
{% endhighlight %}

{% highlight text %}
+ Eintrag 1
+ Eintrag 2
+ Eintrag 3
{% endhighlight %}

{% highlight text %}
- Eintrag 1
- Eintrag 2
- Eintrag 3
{% endhighlight %}

{% highlight text %}
* Eintrag 1
+ Eintrag 2
- Eintrag 3
{% endhighlight %}

Durch alle drei *Markdown*-Beispiele wird folgender HTML-Quelltext erzeugt.

{% highlight html %}
<ul>
<li>Eintrag 1</li>
<li>Eintrag 2</li>
<li>Eintrag 3</li>
</ul>
{% endhighlight %}

### Sortierte/ nummerierte Listen

Bei sortierten/ nummerierten Listen wird als Eintragskennzeichen eine Zahl gefolgt von einem Punkt verwendet. Dabei ist es unerheblich, mit welcher Zahl Sie beginnen oder ob Sie für jeden Eintrag die selbe Zahl verwenden. Sie sollten der Übersichtlichkeit halber aber eine richtige Nummerierung verwenden. Auch weil eventuell in Zukunft eine bestimmte Startnummer von *Markdown* unterstützt wird.

Die folgenden *Markdown*-Beispiele sind also, was den daraus erzeugten HTML-Quelltext angeht, identisch.

{% highlight text %}
1. Eintrag 1
2. Eintrag 2
3. Eintrag 3
{% endhighlight %}

{% highlight text %}
1. Eintrag 1
1. Eintrag 2
1. Eintrag 3
{% endhighlight %}

{% highlight text %}
3. Eintrag 1
3. Eintrag 2
3. Eintrag 3
{% endhighlight %}

Durch alle drei *Markdown*-Beispiele wird folgender HTML-Quelltext erzeugt.

{% highlight html %}
<ol>
<li>Eintrag 1</li>
<li>Eintrag 2</li>
<li>Eintrag 3</li>
</ol>
{% endhighlight %}

### Einrückungen

Sowohl bei unsortierten als auch bei sortierten/ nummerierten Listen können Sie für ein schöneres Textbild den Text von Listeneinträgern umbrechen und einrücken. Das folgende Beispiel zeigt dies exemplarisch.

{% highlight text %}
* Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
  sed diam nonumy eirmod tempor invidunt ut labore et dolore
  magna aliquyam erat, sed diam voluptua.
* At vero eos et accusam et justo duo dolores et ea rebum.
* Stet clita kasd gubergren, no sea takimata sanctus est
  Lorem ipsum dolor sit amet.
{% endhighlight %}

Durch das *Markdown*-Beispiele wird folgender HTML-Quelltext erzeugt.

{% highlight html %}
<ul>
<li>Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
sed diam nonumy eirmod tempor invidunt ut labore et dolore
magna aliquyam erat, sed diam voluptua.</li>
<li>At vero eos et accusam et justo duo dolores et ea rebum.</li>
<li>Stet clita kasd gubergren, no sea takimata sanctus est
Lorem ipsum dolor sit amet.</li>
</ul>
{% endhighlight %}

### Absätze in Listen

Sowohl bei unsortierten als auch bei sortierten/ nummerierten Listen können Sie die einzelnen Einträge als Absätze definieren. Dazu trennen Sie die einzelnen Einträge durch Leerzeilen voneinander ab. Das folgende Beispiel zeigt dies exemplarisch.

{% highlight text %}
* Eintrag 1

* Eintrag 2

* Eintrag 3
{% endhighlight %}

Durch das *Markdown*-Beispiele wird folgender HTML-Quelltext erzeugt.

{% highlight html %}
<ul>
<li><p>Eintrag 1</p></li>
<li><p>Eintrag 2</p></li>
<li><p>Eintrag 3</p></li>
</ul>
{% endhighlight %}