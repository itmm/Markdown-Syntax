---
title: Markdown-Syntax - Überschriften
description: Markdown bietet zwei verschiedene Möglichkeiten, Überschriften auszuzeichnen. Auf dieser Seite werden beide Möglichkeiten beschrieben.
---

## Überschriften

*Markdown* bietet Ihnen zwei verschiedene Möglichkeiten, Überschriften auszuzeichnen. Im Folgenden werden beide Möglichkeiten beschrieben. 

### Möglichkeit 1 (Setext)

Überschriften ersten Grades (`<h1>`) werden durch **Gleichheitszeichen** unter dem Text der Überschrift kenntlich gemacht. Dabei ist es egal, wieviele Gleichheitszeichen Sie verwenden.

{% highlight text %}
Überschrift ersten Grades
=========================
{% endhighlight %}

Hier sehen Sie den HTML-Quelltext, der aus dem vorherigen Markdown-Beispiel erzeugt wird.

{% highlight html %}
<h1 id="berschrift-ersten-grades">Überschrift ersten Grades</h1>
{% endhighlight %}

Wie Sie sehen, wird dabei automatisch der Text der Überschrift etwas aufbereitet und als Wert des `id`-Attributs eingesetzt. Dies ist zum Beispiel dann sinnvoll, wenn Übrschriften Ziele von Springmarken sind. Bei der Aufbereitung des Textes werden leider nur einfache alphanumerische Zeichen zugelassen. In dieser Menge sind zum Beispiel die deutschen Umlaute und das ß nicht mit enthalten und werden einfach weggelassen.

Überschriften zweiten Grades (`<h2>`) werden durch **Bindestriche** unter dem Text der Überschrift kenntlich gemacht. Dabei ist es egal, wieviele Bindestriche Sie verwenden.

{% highlight text %}
Überschrift zweiten Grades
--------------------------
{% endhighlight %}

{% highlight html %}
<h2 id="berschrift-ersten-grades">Überschrift zweiten Grades</h2>
{% endhighlight %}

Weitere Überschriftenebenen (`<h3>` bis `<h6>`) sind mit dieser Variante nicht möglich. Wenn Sie bereits wissen, dass Sie mehr als zwei Ebenen bei den Überschriften benötigen, dann sollten sie von Anfang an auf die nun folgende zweite Möglichkeit setzen.

### Möglichkeit 2 (atx)

Überschriften ersten Grades (`<h1>`) werden durch **eine Raute** am Zeilenanfang kenntlich gemacht.

{% highlight text %}
# Überschrift ersten Grades
{% endhighlight %}

Hier sehen Sie den HTML-Quelltext, der aus dem vorherigen Markdown-Beispiel erzeugt wird.

{% highlight html %}
<h1 id="berschrift-ersten-grades">Überschrift ersten Grades</h1>
{% endhighlight %}

Wie Sie sehen, wird auch bei dieser Variante automatisch der Text der Überschrift etwas aufbereitet und als Wert des `id`-Attributs eingesetzt. Dabei ergibt sich für die deutschen Umlaute das selbe Problem wie berits oben bei der ersten Möglichkeit beschrieben.

Für die nächsten Beispiele sind die erzeugten HTML-Quelltext dementsprechend equivalent und ich werde mir das Notieren dieser hier sparen.

Überschriften zweiten Grades (`<h2>`) werden durch **zwei Rauten** am Zeilenanfang kenntlich gemacht.

{% highlight text %}
## Überschrift zweiten Grades
{% endhighlight %}

Überschriften dritten Grades (`<h3>`) werden durch **drei Rauten** am Zeilenanfang kenntlich gemacht.

{% highlight text %}
### Überschrift dritten Grades
{% endhighlight %}

Überschriften vierten Grades (`<h4>`) werden durch **vier Rauten** am Zeilenanfang kenntlich gemacht.

{% highlight text %}
#### Überschrift vierten Grades
{% endhighlight %}

Überschriften fünften Grades (`<h5>`) werden durch **fünf Rauten** am Zeilenanfang kenntlich gemacht.

{% highlight text %}
##### Überschrift fünften Grades
{% endhighlight %}

Überschriften sechsten Grades (`<h6>`) werden durch **sechs Rauten** am Zeilenanfang kenntlich gemacht.

{% highlight text %}
###### Überschrift sechsten Grades
{% endhighlight %}

Wie Sie sehen, können Sie so alle durch HTML bekannten Überschriftenebenen umsetzen.

Bei dieser Variante können Sie zusätzlich zu den Raute-Zeichen am Anfang der Zeile auch noch Raute-Zeichen nach dem Text setzen. Die Anzahl der Raute-Zeichen am Ende der Zeile muss nicht zwangsläufig mit der Anzahl der Raute-Zeichen am Anfang der Zeile übereinstimmen. Wie gesagt, diese sind optional und nur dafür da, dass es dem ein oder anderen von Ihnen eventuell besser gefällt. Der folgende Quelltext zeigt dies beispielhaft für eine Überschrift dritten Grades.

{% highlight text %}
### Überschrift dritten Grades ###
{% endhighlight %}