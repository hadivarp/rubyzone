---
layout: pages
title: راهنمای نصب
parent: ruby
nav_order: 1
---

# نصب روبی بر روی کامپیوتر

در این قسمت هیچ کد نویسی وجود نداره و فقط آموزشی برای نصب و راه اندازی روبی بر روی کامپیوتر شما . شما باید این مراحل بصورت کامل انجام بدین تا همه چیز درست پیش بره .

`اگر که نمیدونید چطور از ‍‍"PowerShell" در ویندوز ، "Terminal" در مک و "bash" در لینوکس استفاده کنید ، شما نیاز دارین تا اول به قسمت ضمایم در انتها کتاب رفته و کمی در این مورد اطلاعات بدست بیاورید . `


### **MAC**

برای نصب روبی بر روی سیستم عامل مک  مراحل زیر رو به ترتیب انجام بدین  تا نصب کامل بشه :

>از طریق منوی جستجو ترمینال رو باز کنید .
>درون ترمینال دستور `ruby -v` برای پیدا کردن نسخه روبی نصب شده بر روی کامپیوتر وارد کنین

>>>بصورت پیش فرض روبی  نسخه ۲ بر روی کامپیوتر های مک نصب هست

>اگر نسخه ‍‍`ruby` کمتر از "۲" باشه این نسخه خیلی قدیمیه و شما در این مورد سه تا راه دارین :

>> ۱. مورد اول اینکه میتونین سیستم عامل مک دستگاهتون رو به آخرین نسخه بروزرسانی کنین تا ورژن روبی دستگاه شما هم بروزرسانی بشه .

>> ۲. به آدرس `HTTPS://WWW.RUBY-LANG.ORG/EN/DOWNLOADS/` برین و یکی از نسخه های نصبی رو انتخاب کنین .

>> ۳. از یک دوست و یا شخصی که وارده کمک بخواین تا نسخه روبی به نسخه های بالاتر از نسخه فعلی دستگاه شما باشه ارتقا بده .

> ترمینال یک دیرکتوری 'یا محلی برای نوشتن برنامه ها' ایجاد کنین

> از ویرایشگر متن استفاده کنید و فایلهایی با فرمت `rb` درون دیرکتوری ایجاد کنین .

##### نکته:

**دستوراتی از سیستم عامل که شما به اونها زیاد نیاز پیدا میکنین رو خوب یاد بگیرین . این دستورات  فرم قالب همه سیستم عامل هاست و اگه یکی رو بلد باشین توی یاد گرفتن مابقی مشکل چندانی ندارین .**


پس از نصب چیزی که باید توی ترمینال ببینین این شکلیه :


![](/assets/images/macinstall.png)



### **Windows**

> ‍`PowerShell` رو از طریق منوی start پیدا و احرا کنین .

>درون `PowerShell‍` فرمان `ruby -v` رو وارد کنین تا مشخص بشه که آیا روبی رو روی سیستم نصب دارین یا لازمه که اونو  نصب کنین .

>> اگر درون صفحه  `PowerShell` با پیغامه (`ruby is not recognized ..`) مواجه شدین از طریق یکی از دو آدرس زیر اونو نصب کنین .

>>> ۱- http://rubyinstaller.org/

>>> ۲- https://www.ruby-lang.org/en/downloads/.

>>یادتون نره که حتما نسخه ای که از روبی  میخواین نصب کنین حتما  2.0 به بالا باشه .

>> بعد از نصب `PowerShell` ببندین و دوباره باز کنین تا مطمئن بشین همه چی روبهراهه و روبی به درستی اجرا میشه ، اگر هنوز هم مشکلی بود با یکبار `restart` کامپیوتر همه چی حل میشه .

>>حالا باید با اجرای فرمان `ruby -v` نسخه نصب شده از روبی روی کامپیوترتون 2.0 به بالا و نه زیر2.0 باشه .

> ترمینال یک دیرکتوری 'یا محلی برای نوشتن برنامه ها' ایجاد کنین

> از ویرایشگر متن استفاده کنید و فایلهایی با فرمت `rb` درون دیرکتوری ایجاد کنین .





































[اولین برنامه](http://www.localhost:4000/docs/ruby/a_good_first_program){: .btn }
[آموزش روبی](http://localhost:4000/docs/ruby/){: .btn }










<!-- # Typography
{:.no_toc}

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Font stack

By default, Just the Docs uses a native system font stack for sans-serif fonts:

```scss
-apple-system, BlinkMacSystemFont, "helvetica neue", helvetica, roboto, noto, "segoe ui", arial, sans-serif
```

ABCDEFGHIJKLMNOPQRSTUVWXYZ  
abcdefghijklmnopqrstuvwxyz
{: .fs-5 .ls-10 .code-example }

For monospace type, like code snippets or the pre `<pre>` element, Just the Docs uses a native system font stack for monospace fonts:

```scss
"SFMono-Regular", Menlo, Consolas, Monospace
```

ABCDEFGHIJKLMNOPQRSTUVWXYZ  
abcdefghijklmnopqrstuvwxyz
{: .fs-5 .ls-10 .text-mono .code-example }

---

## Responsive type scale

Just the docs uses a responsive type scale that shifts depending on the viewport size. Common elements text elements rendered from markdown use a

| Selector              | Small screen size `font-size`    | Large screen size `font-size` |
|:----------------------|:---------------------------------|:------------------------------|
| `h1`, `.text-alpha`   | 32px                             | 36px                          |
| `h2`, `.text-beta`    | 18px                             | 24px                          |
| `h3`, `.text-gamma`   | 16px                             | 18px                          |
| `h4`, `.text-delta`   | 14px                             | 16px                          |
| `h5`, `.text-epsilon` | 16px                             | 18px                          |
| `h6`, `.text-zeta  `   | 18px                             | 24px                          |
| `body`                | 14px                             | 16px                          |

---

## Headings

Headings are rendered like this:

<div class="code-example">
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
</div>
```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

---

## Body text

Default body text is rendered like this:

<div class="code-example" markdown="1">
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
</div>
```markdown
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
```

---

## Inline elements

<div class="code-example" markdown="1">
Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](another-page).
</div>
```markdown
Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](another-page).
```

---

## Typographic ror

There are a number of specific typographic CSS classes that allow you to do override default styling for font size, font-weight, line height, and capitalization.

[View typography ror]({{ site.baseurl }}{% link docs/ror/ror.md %}#typography){: .btn .btn-outline } -->
