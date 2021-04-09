# SmartNinja Coding Challenges

This is a list of coding challenges that will be regularly updated. If you have an idea for a challenge, create an [issue](https://github.com/smartninja/smartninja-challenges/issues/new) or a pull request in this repository.

You don't need to do challenges in this order. You can pick whichever challenge you like and skip the ones that don't interest you.

Happy coding! 🙂

## 1. Python

### Challenge 1.1: Parse the list of users

#### Basic challenge

In the `data` folder, you can find a file called `users.json`. This file includes (fake) data about 10 people.

Create a Python program that would read the contents of this file and do the following:

- Separate/split the `name` into `first_name` and `last_name`
- For each person print out the following things (in this order):
	- Last name
	- First name
	- Latitude of the city the person lives in (geo/lat)
	- The catch phrase of the company that this person works for

#### Bonus challenge

Create a program that will ask the user to enter some last name (for example "Graham"). If a person with this last name is in `users.json`, then print that person's **name**, **email** and **company name**.

### Challenge 1.2: Parse the weather data

Go to the `data` folder and download the `weather.json` file.

Create a computer program that would read this file and print out the following:

- City name
- Country code
- Current temperature
- Weather description

**Bonus challenge:**

Find values for `sunrise` and `sunset`. This is a timestamp for at which time the sun goes up and at which time goes down (for that specific day).

Convert the timestamps into an actual date and time (day, month, year, hour, minutes).

> Hint: you will need to use the `datetime` library for this.

### Challenge 1.3: Blackjack

Have you ever played Blackjack? If not, try it out, there are plenty of online games out there. The rules are very simple. :)

Write a Blackjack Python script where you can play against the computer.

> **Bonus: Set two levels for computer, aggressive and conservative.** 
> 
> One option is that the player chooses the level for the computer before the game starts. 
> 
> Another option is that the level is set automatically, either before the game or even during the game (the computer could randomly switch from being aggressive to being conservative).

### Challenge 1.4: Print current weather

Create a Python script that you'd run in the Terminal and it would print out the current weather for the given city.

For example, you'd run the script like this:

	python weather.py Berlin,DE

The script would take the input ("Berlin,DE") and call the OpenWeatherMap API to get the weather data for Berlin, Germany (DE means Deutschland, which is a German name for Germany). Then it would print out the weather data in the Terminal.

> Bonus: Create a GUI for your weather program.

### Challenge 1.5: Find tweets

Create a Python script that would find all tweets on a certain keyword that were posted today.

You would run the script like this:

	python tweets.py coding

And the script would print out all the tweets with the "coding" keyword in it (you'll need to use Twitter API for this).

### Challenge 1.6: A Markdown program

Create a Python program (with GUI) that would serve as a Markdown editor. It should look something like [Mou](http://25.io/mou/):

![](http://25.io/mou/img/1@2x.png)

> If you don't know what Markdown is, google it and learn how to use it. You can use [StackEdit](https://stackedit.io/app#) for learning.

## 2. HTML & CSS

### Challenge 2.1: Design implementation

Find some beautiful website design on the web (either search it, or find it on [StartBootstrap](https://startbootstrap.com/themes/) or ThemeForest).

If the design comes with the code implementation, don't copy the code, but instead write the code completely from scratch yourself. When you're done, compare your code to the original.

## 3. Web development

### Challenge 3.1: Blog

Create your own blog. Make sure you implement a text editor, so it's easier for you to make some text bold or insert links etc.

But don't forget about security. All inputs should be validated and cleaned before storing them in the database.

### Challenge 3.2: Task management system

Build a task management system, similar to Asana.com (if you don't know what Asana is, try it out before you start).

You can either make your own personal task management system, or a bigger one where anyone could create their own workspace and invite other people in. It's up to you how complex you'd want this project to be.

Also, you can build the front-end with a simple HTML & CSS & jQuery combo. Or you can use some JavaScript framework (like Vue.js or React) instead. Up to you. :)

### Challenge 3.3: Webshop

Create a webshop with all the necessary features, such as item categories and a checkout.

For a payment system, implement something like Stripe, Gumroad or Braintree, but only use their sandbox environment (for testing purposes) - no need to enable real credit card payments.

### Challenge 3.4: Password management system

Create a password management system, such as Dashlane or LastPass.

> Bonus: also create a Chrome or Firefox plugin with JavaScript.

### Challenge 3.5: Search engine

Create your own search engine. Yes, for real, I'm not kidding. :)

What do you need for a search engine?

1. **A web crawler:** This is basically a background task or a completely separated web app that goes from site to site and clicks all the links and tries to figure out what the website is about.
2. **A search index:** This is just a database of websites. You can use PostgreSQL or MongoDB or something else. Keep it simple. Only store a website name, URL and keywords (that you get from the `<meta>` tag from `<head>`. If that meta tag does not exist, you can analyse the words on the website and get 5 most common words that are not generic words like "and" or "of" (this is optional, although there should be a Python library for that).
3. **A search engine website:** This is a web app where you have a big input box in the middle in which you write a search term and hit enter. Then your web app should check your database (the search index) and find websites that have this keyword.

As you can see, this will be a very simple search engine. No need for a bit more "advanced" stuff like checking how many websites link to a certain site.

### Challenge 3.6: Annotated news

Have you ever heard of a music lyrics website called [Genius](https://genius.com/)? It allows you to **annotate** parts of a music lyric and write comments about it. 

See it for yourself here: [New York, New York by Frank Sinatra](https://genius.com/4576338). Click on the highlighted parts of the text and you'll see comments on the side. This are **annotations**.

For this challenge, create a news web app that would allow users to annotate (comment) certain parts of the text.

P.S.: You'll need a lot of JavaScript here. ;)

## 4. Other

For more coding challenges, try websites like [CodeWars](https://www.codewars.com/) and [HackerRank](https://www.hackerrank.com/).