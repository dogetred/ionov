---
title: Гайд как работать с блогом на gh pages от @doged
date: 2024/1/21
description: View examples of all possible Markdown options.
tag: web development
author: doged
---

# Гайд как работать с блогом на gh pages от @doged

В начале есть несколько пунктов:

> title: Гайд как работать с блогом на gh pages от @doged
> date: 2024/1/21
> description: View examples of all possible Markdown options.
> tag: web development
> author: @doged

В поле `title` нужно указать название поста, в поле `date` - дату, и в поле `description` - описание поста (но не длинное). Остальное тоже можно, но пожеланию, плюсом там особо ничего не меняется по тегам и автору. Если хочешь сделать 

## Вот такой вот заголовок

то просто поставь `##` перед названием

### для заголовка поменьше нужно поставить ###

#### для такого четыре "#", и так далее


## Как сделать всякие хуйни с текстом

**Жирный текст делается двумя звёздочками по обеим сторонам текста**

_такой текст делается с помощью символов `_` с каждой стороны_
например `_sex_`

~~Зачёркнутый текст~~ делается через ~~, пример: `~~sex~~`

Хуйню в начале, где я объяснял про пункты, делалась так: `> хуйня из начала`


## Со списками всё ещё проще, например несортированный список с точками:

- делается
- подстановкой тире в начало каждого пункта
`- хуй`

Cортированный:

1. то же самое
2. но вместо чёрточек - цифры
`3. хуй`

## код в блоге это изи

пишешь в начале три чёрточки ```, потом язык и следом заключительные три чёрточки

```js
export default function Nextra({ Component, pageProps }) {
  return (
    <>
      <Head>
        <link
          rel="alternate"
          type="application/rss+xml"
          title="RSS"
          href="/feed.xml"
        />
        <link
          rel="preload"
          href="/fonts/Inter-roman.latin.var.woff2"
          as="font"
          type="font/woff2"
          crossOrigin="anonymous"
        />
      </Head>
      <Component {...pageProps} />
    </>
  )
}
```

## Таблица

Тут такие пиздорезы, что я в ахуе, но постараюсь объяснить


| **Option** | **Description**                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------- |
| First      | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. |
| Second     | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. |
| Third      | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. |

Такая таблица делается так:
`| **Option** | **Description**                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------- |
| First      | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. |
| Second     | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. |
| Third      | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. |
`

тут бля пиздец, но я надеюсь тебе таблица особо не пригодиться в блоге. А если пригодиться - то пиши мне, попробуем разобраться с этой хуйнёй.

## Ссылка

- [вот такая например](https://nextjs.org)
делается просто:
`[наташа 300 метров куплю пива возьму в рот](https://natribu.org/)`

### футноты

Точечка с ссылочкой сверху как на википедии называется по правильному примечание или футнот. я сам охуел, потому что эту залупу всегда залупой и называл. Но тем не менее эта хуйня делается вот так:

`Залупа [^1].`

А выглядит вот так:
- Залупа [^1].

[^1]: здесь примечание к залупе и делается оно вот так:
`[^1]: примечание к залупе`
Также примечание к залупе поддерживает многопараграфность:

[^2]: пояснение за залупу:

    залупа коня огромная как елда лежащая у роберта под подушкой


# Ну вот собсна и всё, надеюсь тут всё понятно. Юзай на здоровье :)
