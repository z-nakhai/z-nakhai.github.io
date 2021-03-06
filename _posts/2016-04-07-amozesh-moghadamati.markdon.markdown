---
layout: post
title:  "معرفی  markdown"
date:   2016-04-07 01:01:43 +0430
categories: jekyll update
---
**معرفی Markdown**

سایت گیت هاب (github) برای فرمت بندی و قالب بندی متن ها و کامنت ها سینتکسی را معرفی کرده به نام  markdown که ما با استفاده از این سینتکس می توانیم متن ها را Bold کنیم یا مثلا یک لینک داخل متن ایجاد کنیم یا گذاشتن عکس و چیزهای دیگر….
آموزش markdown

آموزش markdown

همانطور که بالا گفتم  موقع گذاشتن کامنت در سایت گیت هاب (github) یک تولبار هم برای ما قرار داده شده تا بتوانیم داخل کامنت خودمون برخی متن ها را Bold یا italic …. کنیم . واقعا دستشون درد نکنه چون بدون این تولبار مجبور بودیم markdown  را یاد بگیریم و اگر می خاستیم متنی را Bold کنیم با یک سینتکس (syntax ) خاصی این کار را انجام دهیم .

قبل از اینکه بریم سراغ آموزش  میخوام سایت زیر رو معرفی کنم.این سایت برای چک کردن کدهای ما است و خروجی کدهامون رو میتونیم راحت ببینیم :

    http://dillinger.io/

خب بریم سراغ قواعد سینتکس markdown :
Headings

برای ایجاد heading (تگ های h1 تا h6) قبل از متن مورد نظرمون از # استفاده می کنیم . مثلا اگر تگ h1 لازم داشته باشیم از یک # قبل از متن استفاده می کنیم , اگر تگ h2 لازم داشتیم از دو تا تگ # استفاده می کنیم و الی آخر ….

مثال :
# The largest heading
## The second largest heading
###### The smallest heading
1
2
3
	
# The largest heading
## The second largest heading
###### The smallest heading

خورجی :
The largest heading
The second largest heading
The smallest headin
Styling text

    برای Bold کردن کلمه یا متن باید دو طرف آن از ** یا __ استفاده کنیم .
    برای Italic کردن کلمه یا متن باید دو طرف آن از * یا _ استفاده کنیم .
    برای Strikethrough (خط خوردگی روی خط ) باید دو طرف آن از~~ استفاده کنیم .

مثال :
**This is bold text**
1
	
**This is bold text**

خروجی :

This is bold text

مثال :
*This text is italicized*
1
	
*This text is italicized*

خروجی :

This text is italicized

مثال : ترکیبی از Bold و Italic
*This text is __extremely__ important*
1
	
*This text is __extremely__ important*

خروجی :

This text is extremely important
Quoting text

برای ایجاد حالت نقل قول یا باید در ابتدای متن یک علامت > قرار دهید .

مثال :
In the words of Abraham Lincoln:

> Pardon my French
1
2
3
	
In the words of Abraham Lincoln:
 
> Pardon my French

خروجی :
آموزش Quoting text

آموزش Quoting text
Quoting code

همانند متن ساده , کدهامونم می توانیم داخل نقل قول بگذاریم تا داخل متن از سایر کلمات متمایز بشوند.برای این کار آنها را باید داخل علامت  backticks بگذاریم .

مثال :
Use `git status` to list all new or modified files that haven't yet been committed.
1
	
Use `git status` to list all new or modified files that haven't yet been committed.

خروجی :
آموزش Quoting code

آموزش Quoting code

اگر بخواهیم چند خط را داخل این نقل قول بگذریم باید از 3 تا ` استفاده کنیم :
Some basic Git commands are:
```
git status
git add
git commit
```
1
2
3
4
5
6
	
Some basic Git commands are:
```
git status
git add
git commit
```

خروجی
آموزش Quoting code

آموزش Quoting code

اون 3 خط رو به اصطلاح highlight میکنه برامون .

بهتر است قبل و بعد از بلاکمون یک خط خالی بگذاریم تا خوانایی  حفظ شود .

مثال :
```
function test() {
  console.log("notice the blank line before this function?");
}
```
1
2
3
4
5
	
```
function test() {
  console.log("notice the blank line before this function?");
}
```

fenced-code-block-rendered

می توانیم مشخص کنید که کدهای مدنظر ما مربوط به کدام زبان برنامه نویسی است تا با رنگ بندی بهتری نمایش یابد .در مثال زیر مشخص کردیم کدهای مدنظر ما مربوط به زبان ruby هست :

مثال :
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
1
2
3
4
5
	
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

خروجی :

format
Links

برای ایجاد لینک در markdown باید متن لینکمان را داخل [] قرار دهیم و خود لینک را داخل () .

مثال :
This site was built using [Alihossein](https://alihossein.ir/)
1
	
This site was built using [Alihossein](https://alihossein.ir/)

خروجی :

This site was built using Alihossein
Lists
Unordered Lists

برای ایجاد لیست های غیرشمارشی باید قبل از هر خط یک علامت * یا – قرار دهیم .

مثال :
- Alihossein Shahabi
- John Adams
- Thomas Jefferson
1
2
3
	
- Alihossein Shahabi
- John Adams
- Thomas Jefferson

خروجی :

    Alihossein Shahabi
    John Adams
    Thomas Jefferson

Ordered Lists

برای ایجاد لیست های شمارشی باید قبل از هر خط عددی  قرار دهیم .

مثال :
1. Alihossein Shahabi
2. James Monroe
3. John Quincy Adams
1
2
3
	
1. Alihossein Shahabi
2. James Monroe
3. John Quincy Adams

خروجی :

    Alihossein Shahabi
    James Monroe
    John Quincy Adams

می توانیم لیست های تودرتو هم درست نماییم . برای این کار باید با قبل از خط مورد نظر 3 تا space بزنیم .

مثال :
1. Push my commits to GitHub
2. Open a pull request
   * Describe my changes
   * Mention all the members of my team
1
2
3
4
	
1. Push my commits to GitHub
2. Open a pull request
   * Describe my changes
   * Mention all the members of my team
خروجی :

    Push my commits to GitHub
    Open a pull request
        Describe my changes
        Mention all the members of my team

Task lists

برای درست کردن لیستی از آیتم ها به همراه checkbox که قابلیت check و uncheck داشته باشند از[ ] و [x]  استفاده می کنیم که اولی برای آیتم هایی هست که check  نشده اند و دومی برای آنهایی که میخواهیم  check  شده باشند:

مثال :
- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed
1
2
3
4
5
	
- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed

خروجی :

    a task list item
    list syntax required
    normalformatting, @mentions, #1234 refs
    incomplete
    completed

Mentioning users and teams

برای mention کردن کاربران دیگر یا گروه های دیگرگیت هاب به کامنت یا بحثتون می توانیم از علامت @ قبل از نام اون اشخاص استفاده کنید .

مثال :
@github/support What do you think about these updates?
1
	
@github/support What do you think about these updates?

Using emoji

شما می توانید داخل متن های خودتون از emoji های گیت هاب هم استفاده کنید .

مثال :
@octocat :+1: This PR looks great - it's ready to merge! :shipit:
1
	
@octocat :+1: This PR looks great - it's ready to merge! :shipit:

خروجی :

emoji-rendered

برای مشاهده لیست کامل emoji هایی که می توانید استفاده کنید به سایت زیر سر بزنید :

    http://www.emoji-cheat-sheet.com/

Paragraphs and line breaks

برای ایجاد پاراگراف فقط کافیست بین متن فعلی و متن بعدی یه خط خالی فاصله باشد .
Lorem
 ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy 
nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.

Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper 
suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem 
vel eum iriure dolor in hendrerit in vulputate velit esse molestie 
consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et 
accumsan et iusto odio dignissim qui blandit praesent luptatum zzril 
delenit augue duis dolore te feugait nulla facilisi.
1
2
3
	
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.
 
Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi.

خروجی :

Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.

Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse molestie consequat, vel illum dolore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi.
Ignoring Markdown formatting

برای اینکه از اجرای برخی کدهای جلوگیری کنید و به Github بگویید آنها را کامپایل نکند (escape) قبل از کد مورد نظر \ قرار میدهیم .

مثال :
Let's rename \*our-new-project\* to \*our-old-project\*.
1
	
Let's rename \*our-new-project\* to \*our-old-project\*.

خروجی :

Let’s rename *our-new-project* to *our-old-project*.
Image Links

برای نمایش عکس از قاعده ی زیر استفاده می کنیم :

![alt text][reference name]

    alt text = متنی که میخواهید برای Alt عکس نمایش یابد.
    reference name = آدرس عکس مورد نظر

مثال :
![Google Logo](https://www.google.com/images/srpr/logo11w.png)
1
	
![Google Logo](https://www.google.com/images/srpr/logo11w.png)

Organizing information with tables

در markdown برای ساخت جدول از | و – استفاده می کنیم .

    برای ساخت هر ستون هدر جدول از – استفاده می کنیم.
    برای جدا کردن مقدار هر ستون از ستون دیگر از  | استفاده می کنیم .

مثال :
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
1
2
3
4
	
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

خروجی :

table-basic-rendered

 