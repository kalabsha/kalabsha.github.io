---
layout: post
title: Ruby Hoedown 2008 Keynote - Chris Wanstrath
---

>本文宗旨：启动一个副业项目，立即投入进去，解决问题。这样你就能够成长。

[GitHub Gist](https://gist.github.com/defunkt/6443)
~~# Video: http://rubyhoedown2008.confreaks.com/08-chris-wanstrath-keynote.html~~

Hi everyone, I'm Chris Wanstrath.

When Jeremy asked me to come talk, I said yes.  Hell yes.  Immediately.  But
then I took a few moments and thought, Wait, why?  Why me?  What am I supposed
to say that's interesting?  Something about Ruby, perhaps.  Maybe the
future of it.  The future of something, at least.  That sounds
keynote-y.

So why don't I just get that part out of the way.  The future of Ruby.

In the future, Ruby will become... more popular.  There will be more
implementations.  There will be more programmers using it.  More
machines with it installed by default.  There will be more people
writing blogs about it, and more people reading blogs about it.

I know this may sound kind of crazy, but you have to trust me.  I'm keynoting.

There will be more RubyGems, and there will be more RubyGems servers.  At
least one, possibly as many as two, and it's conceivable that more
than three new books will be written about it.  Current books will be
released in new editions, with more pages and more in depth information on 
new features.

New Rubyists will be younger, and current Rubyists will get older.  Some
Rubyists will get dogs, others cats.  A few will remain dogless and
catless, perhaps opting for children instead.  (This is a common
mistake, as, in my experience, children are much more expensive than either 
dogs or cats.)

Websites will be created in Ruby, using futuristic versions of Ruby on Rails
and Merb.  Versions like 3.0 and 1.0, respectively.  New web
frameworks will be created with strange names and stranger maintainers.  We will 
come to know _why the lucky stiff as a less violent version of the Joker, matz guys
as a more controlled version of Two Face, Dr Nic as the Penguin (he really loves
fish), and DHH as our Batman.  As for me... I am Iron Man.

New languages will come along, and they will become popular.  People will
continue to scorn Ruby, calling it names like "Python's Perl," or
"Java for nerds," or even, God forbid, "Visual Basic for the web."
(Technically, however, I think that role was already filled by ASP versions 
1 through 3.)

Ruby will be taught in college, to young nubys eager to learn the ways of the
master craftsmen.  Most of the students will be drunk during these
classes, others hungover, all hungry for knowledge.

Behavior will drive us and macros will help define us.  Well, some of us.

Proc.  Lambda.

There will be more conferences.  People will speak at these conferences,
sometimes about Ruby, sometimes not about Ruby. Speakers will wax
philosophically about the glory days of Smalltalk... without actually
having written any Smalltalk.  Others will show benchmarks for their new,
superfast Ruby VM.  No, it's not open source and no, you can't try it
out yet.

Someone will bring up a 2.0 version number, then quickly be hushed.  Suit
people will surround us.  Tests will be mocked, and mocks will be
tested.  Or is that stubs?

Ruby will be fast and it will be slow, patches will be released that break
backwards compatibility, and security vulnerabilities will be handled
in a less than satisfying manner.  Big websites will attract billions
of visitors while little blogs will appear, amaze, then vanish.

Most importantly, Ruby will stay beautiful.  At least, we hope so.

And that's the future of Ruby.

Did that feel keynotey?  Let's talk about the past now.

John von Neumann was one of the great mathematicians of the 20th century.  He
made contributions to cellular automata, set theory, functional
analysis, quantum mechanics, ergodic theory, continuous geometry,
economics and game theory, computer science, numerical analysis, explosive 
hydrodynamics, and statistics.  (I know about 60% of those words.)

He also helped invent the modern computer.  The ones we're all using, right
now.

In the 1940s, von Neumann and a group of, basically, geniuses got together to
build a computer.  It wasn't the first computer, mind you.  In fact,
'computer' is a term once used to describe individuals who computed
numbers.

Charles Babbage was such a computer frustrated by the fallibility of the human
brain - when dealing with massive amounts of numbers, mistakes were
common.  For example, William Shanks spent 15 years calculating 707
digits of Pi.

Tragically, he made a mistake at year 11.  His next four years were
spent computing in vain and only the first 527 digits were correct.

Anyway, Babbage envisioned a machine that could carry out precise instructions
and deliver accurate information. If machines could do physical labor,
why not mental labor?

Guys like Alan Turing got in on the action and came up with ideas which would
eventually produce machines such as ENIAC, the first programmable
digital computer.  While ENIAC was a breakthrough, von Neumann's
architecture was different in an important way: it stored both program 
instructions and user data in RAM.  Prior to von Neumann's ideas, program 
instructions, while modifiable, were stored separately from data.

Like I said, this idea (called the von Neumann or stored-program architecture)
is what we use today.  When you're writing your Rubys in your
TextMates, both the Rubys and TextMates are stored together in RAM.

Having both instructions and data in memory together could be used to
implement, as a primitive example, loops - branch instructions are
modified as the loop iterates.  In the ENIAC and others, these sort of
transformations were done by hand, by programmers.  (Oh, and the first
programmers?  All women.)

Anyway, in the second half of the '40s von Neumann and a small team got
together at the Institute of Advanced Study (IAS) and started working
on a machine based on his stored-program architecture.  To be fair, it
wasn't entirely his idea.  Standing on the shoulders of giants, and all that.
Also, Wikipedia claims that some British team actually beat his team
at implementing a stored-program architecture computer.

But who cares about Wikipedia?

The IAS, where von Neumann's machine was built, was basically a dorm near
Princeton, but not officially affiliated with Princeton, started by
some philanthropists who wanted scientists to stay there, have their
lodging and food paid for, and get their science on.  Big time. Einstein was one
of the first residents, as were von Neumann, Kurt GÃ¶del, and J.
"mother fin'" Robert "atomic bomb" Oppenheimer.

So this place held historians, scientists, and engineers.  The engineers
working with von Neumann on the IAS machine worked in the basement.
Sound familiar?  To this day, the basement is the IAS server room.

These guys working on the IAS machine that summer were both programmers and
engineers.  They would solder the parts themselves, program the
programs, and fix bugs in both hardware and software.  Actually, they
often had a hard time distinguishing between hardware and software bugs.  
Is the code wrong or is the machine wrong?  What a nightmare.

They used about 2300 Radio Shack-caliber vacuum tubes for switches and memory.
Stuff would break constantly.  They'd stay up until 4, 5am drinking
tons of tea with tons of sugar.  In fact, since this was during the
war, sugar was rationed and they were using more than their fair share.  The
historians and other nerds in the IAS building were pretty pissed.
(Sounds like me and my brother over Mountain Dew in high school.)

All the engineers kept notebooks, of course.  Blogs.  They'd write frustrated
entries, only to have massive elated breakthroughs the following day.
Their notes were being sent out to institutes all over the country so
others could reproduce their work and create new machines with the von Neumann 
architecture.

And then they finished.  On June 10, 1952 the IAS machine was fully
operational.  Others built similar machines (though none of the
machines had compatible instruction sets - you couldn't yet write a
portable program) at similar institutions, and the IAS machine then carried 
out its intended purpose:

Help design hydrogen bombs.

The first hydrogen bomb was detonated on November 1, 1952.  It was called "Ivy
Mike," detonated on an island in the Enewetak atoll in the Pacific
Ocean, and was 450 times more powerful than the bomb dropped on
Nagasaki.

So, mathematicians built the first modern computer to aid them in applied
mathematics and hydrodynamics.  These guys were true hackers working
on what was a massive side project, and, in a way, the ultimate yak
shave.

(Interestingly, this may also explain why everyone thinks you need to be great
at math to be a programmer, but I digress.)

Today, that is, in the present, there are a number of high profile
Ruby projects which began as side projects.  Some of them might also
be called... the bomb.

Rubinius now has five people working full time on it, but began humbly
in 2006 as Evan Phoenix's side project.  He wanted to build his own
Ruby.

Ruby on Rails itself was extracted from Basecamp, which was a website
the 37signals guys were doing on the side.  At the time, they were a
design firm and David Hansson was a contractor.

No one really knows what _why does with his time, but Shoes is
certainly moving full steam ahead with no mention of monetary gain.
Just for hack's sake, to make things better for people wanting to put
together GUIs in their favorite langauge, for fun.

Merb started as a pastie, a thin layer on top of Mongrel to allow for
fast, concurrent file uploads.  Developers at Engine Yard now actively
work on the framework.  (Though I'm not so sure it can fit in a single
pastie (or gist) anymore.)

You should always have a side project, too.  Side projects give you an
outlet, provide a useful distraction, let you explore new ideas, learn
new concepts, and generally give you the freedom to be unaccountable.
You don't have to worry about your boss, or your coworkers, or the
damn commentators on Reddit.  Just have some fun.  Treat yourself.

After I dropped out of college, I worked at a PHP shop doing trucking
logistics applications.  We were a broker between independent truckers
and big companies like KMart.  Truckers would register on our website,
say they're going to be in Delaware on the 3rd of May and that they're
heading to Denver, then get information on shipments along their
chosen route.  They could then bid on shipments or accept them, all
through us.

It was a fairly complex application and two things were missing:
version control and constants.  There was no version control, so you'd
have things like main2.php and compute_radius_of_from_shipment7.php
laying around.  Along with versions 0 through 6 of that same file, in
the same directory.  Truly painful.

There were no constants and no configuration, so the source code was
filled with magic numbers.  If you wanted to tweak any of our
algorithms, you had to find the code which did the computation and
change some numbers by hand.  Hopefully the correct numbers.

Naturally, the first thing I did was institutionalize Subversion.
(I've apparently always been a champion of source control, though I
didn't realize it until setting this story to paper.)

The second thing I did was start extracting the magic numbers into
configuration files.  At the time, it was a pretty common PHP idiom to
use .ini files for configuration.  Most of what you'd need was
supported, and I'm pretty sure PHP came with a library (aka a shotgun
blast of functions in the global namespace) that could understand .ini
files.

This worked okay, but once I started tinkering with Rails I was blown
away by YAML.  So clean, so powerful.  There was Syck, the C extension
written by _why, but it was just that: a C extension.  I didn't know
much about loading C code in PHP, and even less about doing it on our
production servers.

So I set out to write a YAML parser in PHP, on my own time.  As a nod
to Syck, I called it Spyc - S P Y C - a simple php yaml class.  It was
my first parser, was stateful, and I think did two passes for the
reference / pointer stuff YAML supports.  It didn't support all of
YAML, but it supported most of it - both dumping and loading.  The
good parts.

I snuck it in and before long we were using YAML with great success at
my company.  Naturally, I put the code up on SourceForge.  King of all
online source code repositories.  My designer friend made a page and
in the first month Spyc was a huge hit.  I swear it had at least 70
downloads.  SEVENTY!

That was a big deal.

Fast forward about nine months: I realized the trucking logistics
business isn't the beacon of progress or congregation of forward
thinking individuals I had envisioned.  After all, they hired me.

I quit and begun re-enrolling in school.  This time I would major in
Computer Science instead of English.  My path was set.

But then, near the end of that summer, a friend IM'd me.  A close
friend I grew up with.  He was into Digg and video games, but was far
from a programmer.  "Hey," he said.  "Do you know MySQL?"

"Shit," I thought.  I figured this conversation would be the modern
day equivalent of said friend asking why Ruby sites are always down.
Real time trolling.

"Yeah, I know MySQL."

"And you know PHP too, right?"

"Yes."  I was dubious about the direction this conversation was headed.

"GameSpot is hiring.  You should apply."

Ah, GameSpot.  He and I were both into video games.  During high
school I worked at a local GameStop, and in college I worked at
EBGames in the mall.  I had all the modern systems and grew up with
Atari, NES, Genesis, all that.

Gamespot.com was a site I had visited quite often while in high school
and college.  By the way, notice how different the names GameSpot and
GameStop are - this would later cause my family endless amounts of
confusion, thinking I had moved to California to work retail.  The
American dream.

So, when you Googled video games, GameSpot was usually #1 or #2 in the
results.  I knew it well.  GameFAQs.com (that's game F A Qs) was owned
by the same company, and probably the site I used most.  It's
basically walkthroughs, how-tos, guides... and cheats.  Lots of
cheats.

Anyway, I had no idea where San Francisco was or what the guys at
GameSpot were looking for, but I applied.  I created a brand new
resume and stayed up all night working on the cover letter.  By the
time I was finished, it was a page long and pretty convincing.

In it I promised to move to California the next day, bringing nothing
but my guitar and Xbox with me.  My family would miss me but I was
ready to leave, and I was hungry to show the world what I could do.
Ready to learn from the masters.

The phone interviews went well, they liked that I was into Macs and
Ruby, and I obviously got the job.  My first time ever stepping foot
in California was when I flew out to find an apartment with my dad.

My work experience wasn't what got me the job.  I'm sure my cover
letter had something to do with it, but my short lived career in
trucking logistics was less than glamorous. I really only had one
thing to show GameSpot - Spyc.  My code was freely available, had been
used in production, and worked.  They could download it and play with
it, or check it out online.  Regardless of whether or not they thought
it was good, they could tell it was clean and well thought out.  Well,
maybe not, but I had a website and 70 downloads.

So I got the job at GameSpot, in my mind the first big step in the
path that brought me right here, thanks to my open source side
project.

Something I learned from that experience is that you don't need to
make money from code to make money thanks to code.  I didn't make
money off Spyc, but I made money thanks to Spyc.  (Also, it got my
name in a book.  But that's a different story.)

So that was pretty cool, and I thought unique, until it happened
again.  While I was working on GameSpot, I was doing more and more
Ruby on the side.  I had an open source Rails tumblelog called
Ozimodo, a crappy FTP server called ftpd.rb (which I used as a way to
learn about threading), and a command line option parser DSL called
Choice.  For Choice, I had a full test suite (I wrote the thing to
learn TDD) and an RDoc generated homepage on Rubyforge.

When CNET, GameSpot's parent company, acquired Chowhound, they decided
to rewrite the site in Rails.  Classic.  They brought on two Rails
programmers from Wayfaring.com and were looking for another. They
found me.

I later found out my RDoc site, Ruby gem, and test suite proved to the
Wayfaring guys I was a "real" Ruby programmer.  They wanted someone
excited about this stuff, and I certainly was.

So they threw a bunch of money in my face and convinced me to work on
Chowhound.  Thanks, again, to open source side projects.

This happened to me twice, so it's not uncommon.  Open source can make
wonderful things happen for you, and not just financially but socially
too.  At Chowhound I met PJ Hyett, a GitHub cofounder and coauthor of
Err the Blog.

So, start a side project.  Who knows where it will take you.

Do you have one now?  If not, why not? Not enough time?  No ideas? I
think I can help with both of those.

First off, the time issue.  I don't know how many of you read RSS, but
I challenge you (that's a keynote term) to give it up for a month.
Just turn it off.  Stop using Google Reader or NetNewsWire or whatever
the kids are using these days.  It's not worth your time.

What should you do instead?  If you use Twitter, try following the
authors of your favorite blogs.  Read their tweets on the bus.  Or in
the bathroom.  Check Ruby Inside once a week and skim over the posts.
Visit an aggregator like planetrubyonrails.com once a month.  But
mainly, let other people do the filtering for you.  Use your time for
other things.

You will not miss out on anything big.  Stuff like the Google App
Engine, or Rubinius running Rails, or the killer speaker line up at
this year's Ruby Hoedown will find its way to you.  How can it not?
I'm willing to bet a lot of the stuff in your RSS reader is stuff you
already knew, or heard about somewhere else.

Personally, I used to check RSS multiple times per day.  Now I don't
use any reader, and haven't since January 2008.

Another big time sink among programmers, I've found, are books on
process and theory.  Books like Smalltalk Best Practice Patterns,
Practices of an Agile Developer, and even, I dare say, the Pragmatic
Programmer, are not worth your time.  Instead, listen to Rein's talk.
Talk to your friends or coworkers.  Let other people filter the
information for you, then decide what you like.

The best way to learn about patterns, idioms, and best practices is to
read open source code.  See how other people are doing it.  It's a
great way to stay current, and it's free.

(I really wish someone had told me this before I bought and read Head
Start Design Patterns.  The whole thing.)

Next implement the Jerry Seinfield GTD method.  Every time you work on
your side project, mark a big X through that day on calendar.
Eventually you'll have a nice line of Xs.  Missing an X will be
torture - it'll mess up your beautiful streak. The goal is to maintain
the streak, even if you don't think you have any ideas for the day.
The best way to overcome writer's block is to write, after all.

Okay, so the time excuse is gone.  Now you have time to work on a side
project and the motivation to do it consistently - the beautiful line
of Xs.  You can devote at least one Sunday a month to it, at least.
But what's the idea?

This is actually the easy part, because you don't need a good idea.
Just start doing something interesting.  Play with a new framework in
Ruby - I hear Sinatra is pretty hot these days.  Learn how to do GUI
stuff, with Shoes.

Learn JavaScript.  Like, for real.  If you don't know what the var,
with, or delete keywords are, get a book and start working on some
flashy effects.  Or download Rhino or Johnson and write some server
side JS.  It's a really beautiful and misunderstood language.

Take some time to master your editor.  Pick up the TextMate book and
dive in.  Write a bundle.  If you're already got massive Vim-fu, try
out Emacs.  Learn why people love it, then use that information in
your holy wars against them.

Write a web service.  Something like Cheat, Subtlety, Disqus, or
TwitPic - tools someone can use to help make running a blog, site, or
coding simpler.  Simple sites that do one thing very well, and surface
their information with digestible APIs.

If you've been meaning to learn a new language, start learning it.
But don't just read a book.  Start writing a program.

Learn Objective-C and Cocoa.  Write a little Mac app to do something
useful, then give it away for free.  Post the code on GitHub.  Put up
a Pledgie badge and accept donations.  Profit.

Write Rake in a Lisp.  It's a good way to learn about metaprogramming
and how command line scripts work in your new language.  Write an RSS
parser and explore native data types in Erlang.  Write a simple blog
and learn about the web frameworks in Haskell.  Write Scrabble in Io,
picking up some OpenGL along the way.  It doesn't matter if people
have done it before.

In fact, stop worrying so much about other people.  Every time I've
worked on a project I thought other people would really love, it was a
massive flop.  Every time I've worked on a project I loved, it worked.
 If you're sitting in this room, your taste is not as far off from
those around you as you'd think.  Build something you love and others
will love it, too.  (Not everyone, of course.)

Alternatively, do something hard, the hardest thing you can think of,
in your language of choice.  Stretch the boundries.  Make Ruby cry out
in pain.  Install ImageMagick.  Rewrite all of the standard library.
Write an Objective-C bridge.  You know, something just devilish.  Flex
your brain.

Work on your small project for a few Sundays, declare it complete then
move on.  Learn another language, or write something else in your new
language.  Pick up a new web framework or work on flashy effect number
two. Add concurrent task execution to your Rake.  The more acclimated
you get to this process, the more creative your ideas will be.  It's
the whole 10% inspiration 90% perspiration thing, and it worked for
me.

This, after all, is how GitHub was started.  Tom and I had full time
gigs, but we'd get together on Saturday, have lunch, then work on
GitHub.  We wanted a pretty and simple way to share Git repositories.
Something we'd use.  Something that would make it easier for us to
share and work on open source.

Now we have three people working on the site full time, thousands of
paying users, and tens of thousands of repositories.

But it wasn't an overnight eureka, and it wasn't intentional.  I
didn't just walk out of high school, pick up a Ruby book, meet Tom and
PJ, then launch the site GitHub.  Before GitHub came, in chronological
order, Spyc, Ozimodo, my ozmm.org tumblelog, ftpd.rb, Choice, Err the
Blog, acts_as_textiled, Cheat!, acts_as_cached, Mofo, Subtlety,
cache_fu, Sexy Migrations, Gibberish, nginx_config_generator, fixture
scenarios builder, Sake, Ambition, and Facebox.  And that's just the
stuff I released.

The more side projects I had, the more I felt the pain of maintaining
open source code.

If you already have a job you love, this doesn't exclude you.  You
probably use, day to day, many side projects from others.  You can
also use your own side projects at your job.  From Emacs configs to
simple web services, there are a ton of things you can do to stretch
your brain.

I had no intention of leaving Chowhound when I wrote Cheat - I just
wanted to make it easier to look up commands I rarely used.  Things
like TwitPic or Twictures have nothing to do with anyone's job,
they're just fun and make life on the Internet a little bit more
enjoyable.  Ruby on Rails may have a financial angle, but if there's
money to be made in Shoes I'm not sure I see it.

My plea to you today is to start a side project.  Scratch your own
itch.  Be creative.  Share something with the world, or keep it to
yourself.

Side projects are less masturbatory than reading RSS, often more
useful than MobileMe, more educational than the comments on Reddit,
and usually more fun than listening to keynotes.

Thank you.

---

The link to the video is now: [Confreaks.TV](http://confreaks.tv/videos/rubyhoedown2008-keynote) or [Youtube](https://youtu.be/e37ggWG_Cig)
