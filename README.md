# HTML Lab, Basic HTML Elements and Document Structure

### Objective
This is will be fairly simple looking, not scale to mobile, have no additional style, and not build anything useful.  It's just stretching your HTML muscles and ability to hit me up for help, or search Google for what you need!  I definitely recommend using the crap out of [W3 Schools](https://www.w3schools.com/html/default.asp) when you're starting out 'cause they have simple examples, list a lot of what you can do, and don't use a lot of technical jargon.  

---
### Requirements

 - Attempt to use your terminal as much as possible to navigate and create stuff on your hard drive!
 - Create a new directory in your `source` directory we made last time, it won't be nested in the first lab I made you do, but rather a sibling. So something like:
```bash
C:/source/
	-- my-first-project/
	-- html-lab/
```
Every time you start a new project or lab I give you, it'll need its own directory, its own `.git` via `git init`, and its own online GitHub repo.
 - Create an `index.html` inside your `html-lab` directory.
 - Use your emmet abbreviation to (*hint* it was the `!` trick you used in the last lab) create your basic HTML structure.
 - Like I mentioned just above, create a new GitHub repo for this lab and call it `html-lab`.
 - Use the TL;DR workflow from the last lab to push your basic `index.html` up to your new GitHub repo.
 - Try to add, commit, and push every ~5 or steps to get used to the flow of pushing a few lines of completed code regularly.  You'll thank me in the future when you have a great working history of your code in your commit history.

---
### Lab

 1. Change the text of your `<title>` element in your document to `HTML Drills`, this will be what the tab displays in your Chrome browser.
 2. Inside the `<body>` of your page, insert `<h1>` through `<h6>` elements, give each heading element some funny text.  These will represent "sections" of the lab.
 3. Add a [comment](https://www.w3schools.com/html/html_comments.asp) before each heading to give yourself a reminder what the purpose of that section should be.
 4. Add a `<p>` element after each heading.  Inside of each `<p>`, write some kind of dank meme.
 5. Add an image after each paragraph on your page.
 6. Wrap each "section" (header, paragraph, image) with a `<section>` element ([hint](https://www.w3schools.com/tags/tag_section.asp)).  You'll need to fix your indenting after wrapping each section.  Struggle like a [goddamn bitch](https://youtu.be/iDNg4UdwmNw) trying to manually adjust it. 
	 - Realize this won't work in large scale projects with dozens of nested elements you wrap and learn the hotkey to `Format Document`.  Right click in your VS Code anywhere and you'll see it in the drop down.  Learn it.  Abuse it.  It's prolly my most used hotkey.
8.  Add an *unordered* list with at least **3** [list items](https://www.w3schools.com/tags/tag_li.asp) in between every paragraph and image.  More dank memes will be each item's text content.
9. Create a form with 3 inputs for first name, last name, and email address. Make sure each input is labeled, and that all of them (not each individually) are wrapped with a form tag.
10. Add a button to the form using an `<input>` tag.  Don't use the `<button>` tag.
	- **Hint**: Whatever asshole decided that an [`<input>`](https://www.w3schools.com/tags/tag_input.asp) tag can also be a button can literally die in a fire.
11. Add an *ordered* list below your final section.  Give the list **5** items that are your Smash Bros. Ultimate tier list opinion.
12. Wrap the entire page in a `<div>`.  Note that you can't add UI Elements anywhere other than the `<body>` of your HTML.  If I see a commit or your repo with a div anywhere other than your HTML body, I'll [kill you](https://www.youtube.com/watch?v=NpOj2BwimrM).
	- I hope you remember your format document hotkey, asshole.  Watch the magic happen.  
13. Add a horizontal line in between each section in your document.
14. Add [hyperlinks](https://www.w3schools.com/tags/tag_a.asp) around each image that opens the image in a new tab.
15. Add a table at the top of your page with the following columns (headers): Month, Day, Year.
16. Add a row for each day you wish you were dead.  I know this would technically be a lot so try and do like **4** rows.
17. Add a hyperlink under the table that links to a good YouTube video.  Just like I've been doing all over this bitch.
18. Add a horizontal line at the bottom of your page.
19. Add a div below that line.
20. Add a `<h1>` inside that div and give it some text content like the title of [your favorite movie](https://www.youtube.com/watch?v=Y5Peo3Nt4eM). 
21. Add an image inside that div and below the header that is the poster of your favorite movie.
22. Add a `<p>` below the movie poster that's a brief description of the cinematic masterpiece that is Kung Pow.
23. Add an unordered list with the cast of the movie.
24. Add another unordered list witht he box office stats, movie budget, and release date.
25. *Embed* a trailer of the movie using YouTube below the lists.  

---

### Boom

Let me know when you get this done by sending me a repo link!  Then we'll move on to *not* making websites that look like ass and learn some CSS to make it look cooler.