
# Cards Against Humanity

## A party game for horrible people.

According to [Wikipedia](https://en.wikipedia.org/wiki/Cards_Against_Humanity)

> [Cards Against Humanity](https://www.cardsagainsthumanity.com/) 
> is an adult party game in which players complete fill-in-the-blank statements 
> using words or phrases typically deemed offensive, risqué or politically 
> incorrect printed on playing cards. 
> It has been compared to the 1999 card game Apples to Apples and originated 
> from a Kickstarter campaign in 2011. 
> Its title refers to the phrase "crimes against humanity", 
> reflecting its politically incorrect content. 

For example, one question is:

  - 🎓 I am sorry Professor, but I couldn't complete my homework because of ___________

and some possible answers are:

  - 👿 The Devil himself.

  - 🐙 A pangender octopus who roams the cosmos in search of love.

  - 👖 Extremely tight pants.

  - 🖤 Racially-biased SAT questions.

  - 🧠 A brain tumor.

  - 😓 Poor life choices.

  - 👨‍👧 Daddy issues.

  - 😷 COVID-19.

  - 🔥 Being on fire.


### The project

We **don't** want you to make an online version of the game; we very much
agree with the game authors when they say 

> We highly recommend not playing online and instead playing in the real world 
> so you can look your dad in the eye while saying "pixelated bukkake."[^0]

Instead we'd just like to use mobile phones (that are ubiquitous) to replace 
the physical deck of cards (that you probably don't carry around all the time)[^1].
But otherwise we'd like to keep as much as possible the spirit and dynamics 
of the original game.

[^0]: Here is the definition of [pixelated](https://en.wikipedia.org/wiki/Pixelation) 😊

[^1]: But by all means, buy the [classic deck of cards](https://www.cardsagainsthumanity.com/products/cards-against-humanity) if you want to support Cards Against
Humanity financially and/or the [Science Pack](https://www.cardsagainsthumanity.com/products/science-pack) whose profits are donated to the [Science Ambassador Scholarship](https://www.scienceambassadorscholarship.org/) for women in STEM.


### Technical stack

  - **Mobile Apps suckz, Web Apps rules.** You app will be hosted in a (mobile)
    browser which means the "usual" foundation: HTML, Javascript, CSS, etc.
    And maybe, if you have been especially naughty, 
    [some](https://mithril.js.org/) 
    [flavor](https://reactjs.org/) 
    [of](https://vuejs.org/) 
    [trendy](https://www.solidjs.com/)
    [framework](https://svelte.dev/) 
    on top of that (?).

  - **Peer-to-peer.** Since every player will use his own mobile phone as a 
    virtual hand of cards, these browser need to communicate. We'd like to
    avoid the need a central server (because, you know, **more work! 🏗️**),
    the [WebRTC](https://webrtc.org/) technology (or a simpler layer on
    top of it, such as [PeerJS](https://peerjs.com/)) could be used.


### FAQ

  - **Is Cards Against Humanity (the company) going to sue me ?**
    Probably not if you're doing it right since they have licensed
    the classic deck of cards under a [Creative Commons License](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode). 👍

  - **But I know only Python, not Javascript!** If you have a problem with
    Javascript, you may try [Pyodide](https://pyodide.org/en/stable/) which
    allows to use the Python langage in the browser. Of course, now you
    have probably probably introduced several much more challenging problems! 🤣 

  - **But I know C++, not Javascript!** Dude/chica, there are limits to what I
    can do 😮‍💨

  - **I couldn't code if my life depended on it, is this project for me?**.
    Do you lack [the proper motivation](https://i.ytimg.com/vi/mWqGJ613M5Y/maxresdefault.jpg)?
    More seriously, learning Javascript -- and a new set of APIs -- will be needed
    and is going to take a bit of time;
    but most of your Python skills should be transferable. And on the other hand,
    it (wildly) guess that it should be "reasonably easy" to get a (very simple) working prototype 
    if you opt for a very simple interface (say, only text and buttons and 
    maybe a complex initial setup to connect to the peers)[^2].
    Of course, there is still plenty of work to do at this point if you want to
    provide a more polished user experience.


[^2]: This statement is highly non-contractual. 😉
