---
title: Tips for coaching a Ruby study group
layout: default
---

# Tips for coaching a Ruby study group

Rails Girls beginners workshops are great at sparking a lot of enthusiasm, and
motivating newcomers to dive deeper, and start learning how to program.

Often times participants of these workshops form Ruby study groups. Here are
some recommendations about how to run such a group as a coach.


## Happiness and fun

Whatever previous experiences and skills they bring, your job as a coach is
to make learning programming as interesting and your group's meetings as fun as
possible. You want your students to be happy when they leave after the meeting:
A little tired, maybe slightly overwhelmed, but always happy.

This can be tough, and you might find yourself suck. Keep learning, try to come
up with better ways, and improve.


## Create a safe space

At our study groups we have found it best to simply make them women-only for
students ("women" meaning everyone who identifies as a woman).

While we wouldn't necessarily be opposed to allow men participate as students,
too, we want these groups to be a great place for women to learn programming,
at their own pace and in their own ways. However, as soon as there's a single
male student dynamics change drastically, and we've found ourselves struggling
at fighting these dynamics and making sure everyone has the best experience
possible.

We've therefor decided to simply not allow men to join the group as students.
They are invited to visit, tag along, or wait for their partners, but they are
asked to find a separate place, and remain silent in order to not disturb the
group.

We recommend to pick up the same policy for your groups, or at least have
a clear policy about who's allowed to join.


## Never call participants girls

Despite the name and branding of the movement that is Rails Girls, as coaches
we never call participants girls.

They may call themselves whatever they like, that's up to them, but as coaches
we call them participants, students, members (of our group), programmers, or
women, depending on the context.

This is should be a no-brainer to you. If it's not, or if have any issues with
this simple rule, we recommend taking a step back, and learn about gender related
issues in our society in general, and tech in particular, before you run a
group. A few great starting points are [here](https://modelviewculture.com),
[here](http://www.ashedryden.com/archive), and [here](http://geekfeminism.wikia.com).


## Be humble: it's not about you

Whatever you do, put the focus on your students. It's about them, not you.

Your job is to help them learn, and end up being thrilled, motivated,
enthusiastic and happy.

Be humble. Put the focus on them, not you.


## Take breaks

However you run the group meetings, take breaks often enough.

Your students will be exhausted much sooner than you are, most of the time, even
though coaching can be extremely exhausting, too.

Make sure to keep an eye on the time that you use for explaing a new concept,
or letting them solve a certain exercise, and take a break early enough.

During the breaks encourage everyone to close their laptops, walk around, chat,
and have some snacks.


## Ask about previous experiences

Often times students who show up at our beginners groups have zero previous
experience with programming. Sometimes they know a little bit of HTML/CSS, made
some modifications to a Wordpress blog, or hacked on a mod for a game. Sometimes
they are or were studying computer science, but find their introductional Java or
Haskell classes suck so much that they're looking for an alternative.

At your very first meeting, and whenever someone joins the group, ask about
their experiences and skills first, as well as their motivation to join the
group. This will give you a few clues about good starting points, and things
they might already be familiar with.


## Keep it as simple as possible

If you are considering coaching a beginners group then you probably are an
experienced developer.

Keep in mind that being a great developer, and being a great teacher and coach
are two very different things, and they require different skills.

Whatever you personally deem interesting, what's your favorite set of tools,
and what kind of programming style you prefer, is a conclusion that you have
drawn after years and years of trying, failing, learning, and trying again.
None of this is relevant to a beginner.

Pick the simplest tools that can be used by everyone on the group in order
to learn about a certain topic. Even if there's a more modern, or more widely
used way to achieve something, consider starting out with teaching the most
basic and simplistic solution.

For example:

* Let them use Sublime or Atom, unless they're already used to a different
  editor (that works well enough as a text based code editor). These work on
  any operating system, and everyone can share shortcuts and editor settings.

* Use the old hashrocket syntax when first explaining hashes: that's one
  unified syntax for all hashes no matter the type of the keys. There's no
  value in knowing two syntaxes when learning the concept, usage, and benefits
  of hashes. Later mention the new syntax, but keep using the old one for at
  least a while.

* The same is true for little used language features. You want your group get
  to the point where they can write useful and interesting code. Many language
  features, even if we use them often, just aren't required for that. Why
  bother introducing for and while loops, lambdas, splats, class variables,
  even conditional assignments, and default arguments. Instead, obey the 80/20
  rule and teach simple code first. Get them to the point where they can write
  their own stuff. You can always introduce more language features later.

* Start teaching tests using `test/unit`: Tests are just methods (which they
  already know), and there's no extra overhead or setup involved. They'll just
  work in Rails, too.

* Build the first web application using Sinatra, not Rails. Introduce HTTP
  and how verbs map to Ruby methods in Sinatra. Then later let them port the
  application to a Rails app.

* Introduce Rails routes without the `resources` DSL. Let them write out each
  one of the routes. This makes it way easier to understand how this compares
  to Sinatra, how the route maps the verb and path to a controller etc.
  Then later explain how Rails has come up with `resources` in order to make
  our lifes easier.

* Introduce migrations by manually crafting migration files, don't use
  generators. Let them number files sequentially (`00`, `01`, etc) as this was
  done in the early days of Rails: This makes it easier to understand the
  naming of the rake tasks `migrate:up` and `migrate:down`. Let them manually
  implement the methods `up` and `down` instead of `change`. Later explain why
  migration files nowadays are timestamped and why there's `change`.


## Break things down

Do not try to teach too much at once. Reduce things. Once you think they're
simple enough, reduce further.

Think hard about what's the least minimum piece of knowledge that does not
require any additional knowledge that hasn't been tought, yet.

Instead of starting out with an entire, fresh Rails application, consider
breaking things down. For example:

* Learn how to write some code that renders a static HTML page manually and
  prints it to the terminal.
* Learn how to save the HTML to a file, so it can be viewed in the browser.
* Learn how to use ERB to render the same HTML.
* Learn how to use Sinatra to serve the file, introducing HTTP.
* Finally learn how to use Rails to render it, introducing routes and
  controllers.

Make sure people understand Ruby basics: What are methods, blocks, classes,
objects? Learning what a method is, how to write your own methods, how
arguments are passed, and mapped to local variables inside the method's
scope, what a scope is, ... all of this might take quite a while for a
newcomer.

Make sure to break down all of this into small, digestible steps.

Keep in mind that, as a programmer, you not only know all of this. You
*breathe* these concepts. You know them so well that you might not even know
how to best explain them. Think about this hard, and try to take the smallest
possible steps, one at a time.

Also, read the chapter "Learning to program" from our book [Ruby For
Beginners](http://ruby-for-beginners.rubymonstas.org).


## Repeat yourself

Learning to program only works through repetition. It is a process of brainwashing
yourself into the ability to recognize patterns, such as a method definition,
and immediately know what it means.

Repeat yourself over and over again. Often times it helps to actually say the
same thing three times, in different ways.

Try to establish memorizable catch phrases, that everyone on the group
memorizes over time. Sentences like: *In Ruby every method always returns
exactly one thing*. Make sure to repeat this often enough, and ask your
students to repeat it. Other examples might be:

* Four things make up a method: a name, a block of code, input (arguments),
  and output (return value).
* A block is a method without a name, passed to another method.
* In Rails, a resource consists of 7 routes.
* A migration represents a change to the database structure.


## Use metaphors

Different people tend to soak up new concepts in different ways.

Try to give precise definitions, but also use metaphors, analogies and images
as much as possible. Try to be playful, but also keep repeating precise
phrases, and *show* how things work.

For example, explain that *A route maps an HTTP verb and a path to a a
controller action. An action is a method on an instance of a controller class
that route maps to.* Then also come up with a metaphor, e.g. *A route is like
the receptionist in a hotel: The browser's request walks up to them, and is
being sent to a particluar floor and room number.* Or: *A route is like the
waiter in a restaurant. They take your order, and bring it to the right chef,
depending on the dish you ordered.*

Also consider trying more creative learning methods:

As part of their homework, ask them to come up with a little comic that turns a
metaphor into a story.  Conduct a little role playing game or play where
different people play roles of two or three classes, passing around data in the
form of pieces of paper. Ask the group to come up with good ideas to represent
some simple piece of code that you've been working on together. Let them look
around and identify things that could be implemented as classes: pretty sure
there's a `Lamp` that could have a method `toggle` to be switched `on` and
`off`. We've once implemented a couple classes `WaffleIron`, `Dough` and
`Waffle`, then conducted a role playing game with these.


## Observe and listen, be flexible

Since everyone's different there won't ever be two classes or groups where
everything works well the same way. You'll need to continuously adapt to your
students and the group's dynamics.

No matter how extrovert you normally are, try to observe and listen as much
as possible. Your students' body language gives you clues about how they
feel, how well an explanation worked for them, and how to proceed.

Try to be flexible and adjust to the group, and every student individually.

Experiment with, and mix different styles of teaching, like

* Do lecture-style classes where you explain and demonstrate concepts on a
  shared screen or projector
* Let students pair up, and solve small exercises
* Let the entire group work conduct a role playing game, or brainstorm ideas
  for a story or comic about a small piece of code
* Let them brainstorm and discuss ideas for things that could be represented
  as, e.g. hashes, nested arrays, objects
* Let students research a certain, small topic during the week and then present
  about it during your group meeting

You may want to do more lecture style classes in the very beginning, explaining
basic programming concepts, while the group is still very new. Make sure to add
in more and more longer sessions where they do exercises, ideally in pairs, but
also, sometimes, on their own. Make sure to add in sessions where the group
works on something on their own, and completely walk away for a little while.


## Be patient

Especially when this is your first group you'll need to be extra careful to be
patient. Super extra patient.

You have completely internalised all the knowledge that makes up entire books
about learning programming. All of this sits in your mind, ready for you to
be used without thinking about it further.

Students who never learned any programming on the other hand will be
overwhelmed in not time when you try to explain too much at once. Also, it simply
takes a little while, and quite some repetition, in order for a certain concept
to trickle in, and be well known enough to be *used* while thinking about
something else (like, thinking about the next concept, or how to solve a
certain exercise *using* that concept).


## Make zero assumptions

Even though impossible, try to make zero assumptions.

When someone has a hard time figuring out a certain error raised in their code
then do not assume they've read the error message carefully, or had a look at
the backtrace. Instead ask. If the error has to do with an array, do not assume
they understand what an array is, instead ask.

Do not assume that, once you've given a definition for a certain concept, like
MVC, and they can repeat it, they also are able to properly use it. Instead ask
where they think a piece of code should fit in, and try to come up with helpful
answers.


## Summarize, give the bigger picture

Try drilling down into the details often enough so your students understand
every little step that happens when an object is instantiated, a method is
called, arguments passed and assigned to local variables, and eventually a
return value is returned.

However, also try to always embed things into a bigger picture. Have a big
picture roadmap for your group curriculum. After each week's meeting summarize
what they've learned, and how far they've come in the overall roadmap.

When doing their first steps in a Rails app, trying to figure out a certain
feature, don't forget to always also summarize things, and talk about the
end-to-end process that a request/response cycle goes through.


## Be positive, praise progress

Everyone is always doing the best they can. Whatever progress your students
make, be sure to give positive feedback, and compliment the progress they've
made.

Maybe things are going a little bit slower than you expected, or maybe they
take a different route. That's still progress, and it's great they've made
it this far. Be sure to give positive feedback.

Also, often times students aren't really aware about the progress they're
actually making:

For example, after introducing what a method is, and explaining how they are
defined, and used, your students might feel overwhelmed and confused. Just a
few weeks later they'll define and use their own methods as if they always knew
them. However, because the exercises they're currently working on also might
feel a little overwhelming, they feel they haven't made any progress
whatsoever.

Be sure to point out how much progress they've already made, and how proud they
should feel.


## Have weak opinions

Let's face it, the Ruby community values "strong opinions" a lot, and everyone
has their own. This is probably beneficial to the community as a whole: lots
of discussions ensue, and everyone hopefully comes out wiser than before.

However, as a beginner, you're usually better off not limiting yourself to any
such opinion exclusively. Instead you would ideally look at many different
solutions, hear lots of different opinions, and try to make up your mind,
basically catching up on a decades evolutionary learning process that the
community has gone through as a whole.

Since your students will look at you, and value your guidance, you should try
and take a step back: Have weak opinions.

Even if you very much prefer one tool over another, one editor over another,
one whatever thing over another one, remain silent about your opinions. Instead
give a list of possible solutions, mention some of the benefits and drawbacks,
and explain the choice you've potentially made for the current group or
curriculum.  Ideally, if possible, let them decide and pick the solution they
want to go with, and ask for their reasons.

You want your students to remain curious and open-minded. For example, if
you happen to really dislike Cucumber for whatever reasons, if your group
or individual students happen to be excited about it, then you want to fuel
their curiosity, instead of discouraging it. If they want to use Bootstrap,
maybe because a friend has used it before, encourage them to try it out, even
if you feel there are better solutions.


## Never cancel a group meeting

Try as hard as possible to never cancel a group meeting. Make sure someone
else can take over if you're travelling, or sick. Run the meeting even if
there's only a single attendee.

It helps to grow the group big enough, and have enough coaches, so that
there's always a group of at least 3-4 people attending.

This gives stability, predictability, and builds trust, which in turn helps
your students stay motivated. If you cancel meetings too often you might
eventually blast your group.


## Build an identity

Once the group is somewhat established, people got to know each other,
and had a bunch of great meetings, having lots of fun, ask them to come
up with a name for the group.

Let them set up a mailinglist, maybe a Twitter account, or Facebook page. Set
up a GitHub organization with them, and add everyone as an admin. Use
repositories for discussions, documents and code examples. Should someone be
uncomfortable committing in public then ask GitHub for a free organizational
account with private repositories.


## Give long term perspectives

Give your group long term perspectives.

Explain that they'll very soon be able to write Ruby scripts which might
be simple, but very useful. E.g. if they're working with CSV files a lot
at work, they'll now be able to write a simple script in order to extract
certain things, instead of doing painful, repetitive manual work.

Tell them when they can expect to be able to build their first web
applications, when you think they'll be ready to apply for a job as a junior
programer.

Also be sure to tell them about Rails Girls Summer of Code, a project that
dedicately aims at providing a longer term goal for study groups to aim at.


## Encourage them to join other events

Even for beginners it often times is a great experience to join a local Ruby
meetup once in a while, join a hackday (ask the whole group to participate and
work on their shared learning project for a day), or visit a local conference
(ask the conference organizers about free tickets, student discounts, or
whether you could join with them for a just few talks for free).

Even if they don't fully understand every technical talk, it can be inspiring
to them to listen to the talks, talk to developers about their experiences, or
just enjoy the nice atmosphere and have fun.


## Invite guest stars and experts

When well know programmers visit your city invite them to visit your group,
and maybe give a short lecture on a certain topic. Should your group be
interested in a certain topic that you don't excell in, invite an expert
to give a training session or two.

Having Konstantin Haase visit and do an introductional session about HTTP can
be priceless. Not only will they get a great introduction, feel honored about
being given this opportunity, and get to know a brilliant programer. They'll
also be able to enjoy watching everyone's jawbones drop when mentioning it
casually at their first conference ... which can help boost self-esteem, too
(not even kidding).


## Educate yourself

Coaches often times are seasoned developers, often times male, and priviledged
enough to be able to spend their time coaching a group regularly.

If you fall into this group make sure to spend enough time educating yourself
about some of the issues you'll want to pay attention towards. Some starting
points:

* [So you want to be an ally](http://juliepagano.com/blog/2014/05/10/so-you-want-to-be-an-ally/) by Julie Pagano
* [Resources for allies](http://geekfeminism.wikia.com/wiki/Resources_for_allies) on Geekfeminism
* [Micro agressions](https://modelviewculture.com/pieces/where-are-you-really-from-microaggressions-and-making-tech-meetups-safe) by Nasma Ahmed
* [Imposter syndrom](http://geekfeminism.wikia.com/wiki/Impostor_syndrome) on Geekfeminism
* [Stereotype threat](http://en.wikipedia.org/wiki/Stereotype_threat) on Wikipedia, and [How it works](http://www.explainxkcd.com/wiki/index.php/385:_How_it_Works) by xkcd.
* [Straight white male](http://whatever.scalzi.com/2012/05/15/straight-white-male-the-lowest-difficulty-setting-there-is/) by John Scalzi
* [It's everywhere](http://www.sinfest.net/view.php?date=2011-10-09) by Tatsuya Ishida

