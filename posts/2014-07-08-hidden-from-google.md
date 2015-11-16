## Hidden From Google

##### The making of [HiddenFromGoogle.com](http://hiddenfromgoogle.afaqtariq.com)

---

#### A Little Background

Like many web developers I love what I do and try to keep learning and building useful web applications every minute that I can. That is why last weekend, like any weekend, I got home from work, picked a new web technology that I want to learn, picked an idea which I consider personally useful or interesting and began building a website. Except, this time, it would lead to the simplest web project I ever created and also the most contraversial.

The technology I was trying to experiment with was AngularJS. My co-worker, Joe (Hi Joe!), had shown me how powerful the tiny front-end framework could be and I just could not wait to try it out. As for the idea, I looked to Google News for inspiration. The story which grabbed my attention was the EU “Right to be Forgotten” ruling.

#### Why this idea?

The ruling mandated that Google censor links on its search engine upon request from individuals. I never have been an advocate for privacy and do not have a strong opinion on the matter. The reason the story stood out to me was because several media outlets had started publishing articles to announce receipt of a Google “Right to be Forgotten” censorship notice. This seemed inefficient to me. I did not want to read countless articles over the course of the next year detailing receipt of each censorship letter from Google by each media outlet. I simply wanted to see a list of links which were the subject of current or future censorship. I felt that it was important information which would help me understand what kind of requests were being made and by whom. And creating such a list seemed straightforward since the ruling only applied to Google’s EU domains.

For those not interested in technical details, skip the next section.

#### Technical Details

Now that I had an idea which interested me I went ahead and started finding links manually on Google News. I collected roughly 10 links initially and started to verify them one by one. I would take search terms suggested by the article(s) and search it on Google.com, Google.de, and Google.co.uk. Comparing the results between domains, I started to see evidence of missing links from Google’s EU domains’ search results. After the first few, I remembered that I can limit Google searches to specific domains via a “site:” qualifier. This made the sped up the process as I only had to go through a few pages of Google results. In a few minutes, I had come away with a list of links which passed the process.

Now, it was time to set up the webpage. A simple Ctrl-C and Ctrl-V of the free Bootstrap MAXCDN links for a Bootswatch theme and suddenly I had a beautiful page in front of me. The idea was to take the list of links, along with a few addendum details, and place it into a JSON object. Then, I wanted to see if I could repeat what Joe had blown my mind with earlier that day. Very quickly, I was able to turn the JSON object into a table of links through the magic of ng-repeat. Next, I added an input box above the table to act as a search filter. The remainder of the night involved tinkering with different aspects of Angular, including custom directives like ng-Table.

#### The Birth of HiddenFromGoogle

After I had a working page, I stepped away for a few hours to give my eyes a break. I often find myself resisting taking breaks while learning something new. And like many times before, taking a break allowed me to gather my thoughts and reflect. While I was away from my laptop I realized that even though the page had served its purpose of teaching me introductory Angular, it might be useful to others who wish to contribute and add to the list of links. It was definitely an important and relevant topic in the web development community.

I started to feel excited and wanted to return to my Chromebook to publish the webpage. I went back to my terminal window to the remote VM and started to strip the page of some unnecessary features and code. I even ventured over to GoDaddy and bought a new domain. My Girlfriend was not happy about this; I was now eating into next month’s “Afaq’s Tech Expenses” budget.

About 30 minutes later, [HiddenFromGoogle.com](http://hiddenfromgoogle.afaqtariq.com) was up and running. I submitted it to Reddit and Hacker News and stepped away from my laptop, trying to convice myself that this time, I would not code for the remainder of the weekend. Within a few hours, the site had gone all the way to #1 on Hacker News, though it did not stay there for long. Impressed by the Google Analytics showing hundreds of views on the site, I felt motivated to return to some coding. Through the next few days, the site gained more attention and incited some interesting discussions and debates.

#### First Few Days

The Disqus thread attracted comments from both sides of the spectrum of privacy rights. Some hated the site and felt it was a detriment to a ruling which supported privacy of an individual, which they felt was severely lacking on the wild-west Internet. Others felt it was a healthy reaction to the ruling in the EU and allowed us to see instances in which the law was being used to hide important public information about some people’s pasts. One person on the Hacker News thread asked why a micro-website like [HiddenFromGoogle.com](http://hiddenfromgoogle.afaqtariq.com) was loading so much JavaScript. I realized that I was still loading Angular, which did not seem to serve a purpose anymore. I removed Angular from the page.

A few reporters had reached out to learn more about HiddenFromGoogle. I naively asked my friend if she had ever head of a publication called “Vice magazine”. I told her that I had never heard of them and that some guy had reached out and wanted to talk about HiddenFromGoogle. I ended up doing that interview and the others which followed. Each time, I reiterated the story of the site, tried to focus on how the webpage is not meant to take sides but instead focus on providing information for people to make up their own minds on the subject. I also made it a point to mention that, personally, I did not have a strong opinion on the matter. I was very weary of creating people believing that I felt one way or another about the subject. The strongest opinion I had formed after creating HiddenFromGoogle was that Angular was an awesome and efficient technology.

In one weird instance, someone who works at a large, reputable news organization emailed me a tirade on how “wrong” the site is, how immoral it is, and how he knows people who are ready to sue me. To be fair, he did make some good points about validity of data on the site. That was probably the oddest of the emails (so far).

#### Main Takeaways

**So what did I learn from all of this?**

I love web development because it allows me to create things which can be beneficial to myself and others. When I share one of my ideas/creations with the world and it gets a little bit of attention, I need to be prepared. HiddenFromGoogle has been hated on, evangelized, and misinterpreted. The best thing I can do is: know why I am doing it and repeat it often. I should publish my ideas sooner rather than later.

**What do I want people to take away from all of this?**

The purpose of HiddenFromGoogle was always to allow people to see links which Google had served censorship letters for. The site is a source of information to help you make up your own mind. I haven’t made up my mind on whether the EU “Right to be Forgotten” ruling is helpful or hurtful to the web. There are very good arguments and cases on both sides of the spectrum which deserve thorough (civil) debate. What we decide as a society will help define how the information on the Internet should be treated. I am very curious to see how this debate plays out over the next few years.

AngularJS is awesome. You should use it.