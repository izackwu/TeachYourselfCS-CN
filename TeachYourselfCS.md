# Teach Yourself Computer Science

If you’re a self-taught engineer or bootcamp grad, you owe it to yourself to learn computer science. Thankfully, you can give yourself a world-class CS education without investing years and a small fortune in a degree program 💸.

There are plenty of resources out there, but some are better than others. You don’t need yet another “200+ Free Online Courses” listicle. You need answers to these questions:

*   **Which subjects** should you learn, and why?
*   What is the **best book or video lecture series** for each subject?

This guide is our attempt to definitively answer these questions.

## TL;DR:

Study all nine subjects below, in roughly the presented order, using either the suggested textbook or video lecture series, but ideally both. Aim for 100-200 hours of study of each topic, then revisit favorites throughout your career 🚀.

| Subject                                           | Why study?                                                                                                                                | Best book                                               | Best videos                       |
|---------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------|-----------------------------------|
| **[Programming](#programming)**                   | Don’t be the person who “never quite understood” something like recursion.                                                                | _Structure and Interpretation of Computer Programs_     | Brian Harvey’s Berkeley CS 61A    |
| **[Computer Architecture](#architecture)**        | If you don’t have a solid mental model of how a computer actually works, all of your higher-level abstractions will be brittle.           | _Computer Organization and Design_                      | Berkeley CS 61C                   |
| **[Algorithms and Data Structures](#algorithms)** | If you don’t know how to use ubiquitous data structures like stacks, queues, trees, and graphs, you won’t be able to solve hard problems. | _The Algorithm Design Manual_                           | Steven Skiena’s lectures          |
| **[Math for CS](#math)**                          | CS is basically a runaway branch of applied math, so learning math will give you a competitive advantage.                                 | _Mathematics for Computer Science_                      | Tom Leighton’s MIT 6.042J         |
| **[Operating Systems](#operating-systems)**       | Most of the code you write is run by an operating system, so you should know how those interact.                                          | _Operating Systems: Three Easy Pieces_                  | Berkeley CS 162                   |
| **[Computer Networking](#networking)**            | The Internet turned out to be a big deal: understand how it works to unlock its full potential.                                           | _Computer Networking: A Top-Down Approach_              | Stanford CS 144                   |
| **[Databases](#databases)**                       | Data is at the heart of most significant programs, but few understand how database systems actually work.                                 | _Readings in Database Systems_                          | Joe Hellerstein’s Berkeley CS 186 |
| **[Languages and Compilers](#languages)**         | If you understand how languages and compilers actually work, you’ll write better code and learn new languages more easily.                | _Compilers: Principles, Techniques and Tools_           | Alex Aiken’s course on Lagunita   |
| **[Distributed Systems](#distributed-systems)**   | These days, _most_ systems are distributed systems.                                                                                       | _Distributed Systems, 3rd Edition_ by Maarten van Steen | MIT 6.824                         |

## Why learn computer science?

There are 2 types of software engineer: those who understand computer science well enough to do challenging, innovative work, and those who just get by because they’re familiar with a few high level tools.

Both call themselves software engineers, and both tend to earn similar salaries in their early careers. But Type 1 engineers grow in to more fulfilling and well-remunerated work over time, whether that’s valuable commercial work or breakthrough open-source projects, technical leadership or high-quality individual contributions.

> The global SMS system does around 20bn messages a day. WhatsApp is now doing 42bn. With 57 engineers. [pic.twitter.com/zZrtSIzhlR](https://t.co/zZrtSIzhlR)
> 
> — Benedict Evans (@BenedictEvans) [February 2, 2016](https://twitter.com/BenedictEvans/status/694342874729545729)

Type 1 engineers find ways to learn computer science in depth, whether through conventional means or by relentlessly learning throughout their careers. Type 2 engineers typically stay at the surface, learning specific tools and technologies rather than their underlying foundations, only picking up new skills when the winds of technical fashion change.

Currently, the number of people entering the industry is rapidly increasing, while the number of CS grads is essentially static. This oversupply of Type 2 engineers is starting to reduce their employment opportunities and keep them out of the industry’s more fulfilling work. Whether you’re striving to become a Type 1 engineer or simply looking for more job security, learning computer science is the only reliable path.

> Lol oh but they were.... [pic.twitter.com/XVNYlXAHar](https://t.co/XVNYlXAHar)
> 
> — Jenna Bilotta (@jenna) [March 4, 2017](https://twitter.com/jenna/status/838161631662092289)

## Subject guides

### Programming

Most undergraduate CS programs start with an “introduction” to computer programming. The best versions of these courses cater not just to novices, but also to those who missed beneficial concepts and programming models while first learning to code.

Our standard recommendation for this content is the classic _Structure and Interpretation of Computer Programs_, which is available online for free both as [a book](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html), and as a set of [MIT video lectures](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/). While those lectures are great, our video suggestion is actually [Brian Harvey’s SICP lectures](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter) (for the 61A course at Berkeley) instead. These are more refined and better targeted at new students than are the MIT lectures.

We recommend working through at least the first three chapters of SICP and doing the exercises. For additional practice, work through a set of small programming problems like those on [exercism](http://exercism.io).

For those who find SICP too challenging, we recommend _[How to Design Programs](http://www.htdp.org/)_. For those who find it too easy, we recommend _[Concepts, Techniques, and Models of Computer Programming](https://smile.amazon.com/Concepts-Techniques-Models-Computer-Programming/dp/0262220695/)_.

### Computer Architecture

Computer Architecture—sometimes called “computer systems” or “computer organization”—is an important first look at computing below the surface of software. In our experience, it’s the most neglected area among self-taught software engineers.

_The Elements of Computing Systems_, also known as “Nand2Tetris” is an ambitious book attempting to give you a cohesive understanding of how everything in a computer works. Each chapter involves building a small piece of the overall system, from writing elementary logic gates in HDL, through a CPU and assembler, all the way to an application the size of a Tetris game.

We recommend reading through the first six chapters of the book and completing the associated projects. This will develop your understanding of the relationship between the architecture of the machine and the software that runs on it.

The first half of the book (and all of its projects), are available for free from [the Nand2Tetris website](http://www.nand2tetris.org). It’s also available as [a Coursera course with accompanying videos](https://www.coursera.org/learn/build-a-computer).

In seeking simplicity and cohesiveness, Nand2Tetris trades off depth. In particular, two very important concepts in modern computer architectures are pipelining and memory hierarchy, but both are mostly absent from the text.

Once you feel comfortable with the content of Nand2Tetris, our next suggestion is Patterson and Hennessy’s _[Computer Organization and Design](https://smile.amazon.com/Computer-Organization-Design-Fifth-Architecture/dp/0124077269)_, an excellent and now classic text. Not every section in the book is essential; we suggest following Berkeley’s [CS61C course](http://inst.eecs.berkeley.edu/~cs61c/sp15/) “Great Ideas in Computer Architecture” for specific readings. The lecture notes and labs are available online, and past lectures are [on the Internet Archive](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_).

[![Elements of Computing Systems](https://teachyourselfcs.com/elements-computing-systems.jpg)](http://www.nand2tetris.org) 

> Hardware is the platform
>
> — Mike Acton, Engine Director at Insomniac Games
> ([watch his CppCon talk](https://www.youtube.com/watch?v=rX0ItVEVjHc))

### Algorithms and Data Structures

We agree with decades of common wisdom that familiarity with common algorithms and data structures is one of the most empowering aspects of a computer science education. This is also a great place to train one’s general problem-solving abilities, which will pay off in every other area of study.

There are hundreds of books available, but our favorite is _[The Algorithm Design Manual](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/)_ by Steven Skiena. He clearly loves this stuff and can’t wait to help you understand it. This is a refreshing change, in our opinion, from the more commonly recommended Cormen, Leiserson, Rivest & Stein, or Sedgewick books. These last two texts tend to be too proof-heavy for those learning the material primarily to help them _solve problems_.

For those who prefer video lectures, [Skiena generously provides his online](https://www.youtube.com/watch?v=A2bFN3MyNDA&list=PLOtl7M3yp-DX32N0fVIyvn7ipWKNGmwpp). We also really like Tim Roughgarden’s course, available from Stanford’s MOOC platform Lagunita, or [on Coursera](https://www.coursera.org/specializations/algorithms). Whether you prefer Skiena’s or Roughgarden’s lecture style will be a matter of personal preference.

For practice, our preferred approach is for students to solve problems on [Leetcode](https://leetcode.com). These tend to be interesting problems with decent accompanying solutions and discussions. They also help you test progress against questions that are commonly used in technical interviews at the more competitive software companies. We suggest solving around 100 random leetcode problems as part of your studies.

Finally, we strongly recommend _[How to Solve It](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/)_ as an excellent and unique guide to general problem solving; it’s as applicable to computer science as it is to mathematics.

[![The Algorithm Design Manual](https://teachyourselfcs.com/skiena.jpg)](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/) [![How to Solve It](https://teachyourselfcs.com/polya.jpg)](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/) 

> I have only one method that I recommend extensively—it’s called think before you write.
>
>— Richard Hamming

### Mathematics for Computer Science

In some ways, computer science is an overgrown branch of applied mathematics. While many software engineers try—and to varying degrees succeed—at ignoring this, we encourage you to embrace it with direct study. Doing so successfully will give you an enormous competitive advantage over those who don’t.

The most relevant area of math for CS is broadly called “discrete mathematics”, where “discrete” is the opposite of “continuous” and is loosely a collection of interesting applied math topics outside of calculus. Given the vague definition, it’s not meaningful to try to cover the entire breadth of “discrete mathematics”. A more realistic goal is to build a working understanding of logic, combinatorics and probability, set theory, graph theory, and a little of the number theory informing cryptography. Linear algebra is an additional worthwhile area of study, given its importance in computer graphics and machine learning.

Our suggested starting point for discrete mathematics is the set of [lecture notes by László Lovász](http://www.cs.elte.hu/~lovasz/dmbook.ps). Professor Lovász did a good job of making the content approachable and intuitive, so this serves as a better starting point than more formal texts.

For a more advanced treatment, we suggest _[Mathematics for Computer Science](https://courses.csail.mit.edu/6.042/spring17/mcs.pdf)_, the book-length lecture notes for the MIT course of the same name. That course’s video lectures are also [freely available](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/), and are our recommended video lectures for discrete math.

For linear algebra, we suggest starting with the [Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) video series, followed by Gilbert Strang’s [book](https://www.amazon.com/Introduction-Linear-Algebra-Gilbert-Strang/dp/0980232775/) and [video lectures](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/video-lectures/).

> If people do not believe that mathematics is simple, it is only because they do not realize how complicated life is.
>
>— John von Neumann

### Operating Systems

_[Operating System Concepts](https://www.amazon.com/dp/1118063333/)_ (the “Dinosaur book”) and _[Modern Operating Systems](https://www.amazon.com/dp/013359162X/)_ are the “classic” books on operating systems. Both have attracted criticism for their writing styles, and for being the 1000-page-long type of textbook that gets bits bolted onto it every few years to encourage purchasing of the “latest edition”.

_Operating Systems: Three Easy Pieces_ is a good alternative that’s [freely available online](http://pages.cs.wisc.edu/~remzi/OSTEP/). We particularly like the structure of the book and feel that the exercises are well worth doing.

After OSTEP, we encourage you to explore the design decisions of specific operating systems, through “{OS name} Internals” style books such as _[Lion's commentary on Unix](https://www.amazon.com/Lions-Commentary-Unix-John/dp/1573980137/)_, _[The Design and Implementation of the FreeBSD Operating System](https://www.amazon.com/Design-Implementation-FreeBSD-Operating-System/dp/0321968972/)_, and _[Mac OS X Internals](https://www.amazon.com/Mac-OS-Internals-Systems-Approach/dp/0321278542/)_.

A great way to consolidate your understanding of operating systems is to read the code of a small kernel and add features. A great choice is [xv6](https://pdos.csail.mit.edu/6.828/2016/xv6.html), a port of Unix V6 to ANSI C and x86 maintained for a course at MIT. OSTEP has an appendix of potential [xv6 labs](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf) full of great ideas for potential projects.

### Computer Networking

Given that so much of software engineering is on web servers and clients, one of the most immediately valuable areas of computer science is computer networking. Our self-taught students who methodically study networking find that they finally understand terms, concepts and protocols they’d been surrounded by for years.

Our favorite book on the topic is _[Computer Networking: A Top-Down Approach](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/)_. The small projects and exercises in the book are well worth doing, and we particularly like the “Wireshark labs”, which they have [generously provided online](http://www-net.cs.umass.edu/wireshark-labs/).

For those who prefer video lectures, we suggest Stanford’s [_Introduction to Computer Networking course_](https://lagunita.stanford.edu/courses/Engineering/Networking-SP/SelfPaced/about) available on their MOOC platform Lagunita.

The study of networking benefits more from projects than it does from small exercises. Some possible projects are: an HTTP server, a UDP-based chat app, a [mini TCP stack](http://jvns.ca/blog/2014/08/12/what-happens-if-you-write-a-tcp-stack-in-python/), a proxy or load balancer, and a distributed hash table.

> You can’t gaze in the crystal ball and see the future. What the Internet is going to be in the future is what society makes it.
>
>— Bob Kahn

[![Computer Networking: A Top-Down Approach](https://teachyourselfcs.com/top-down.jpg)](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/) 

### Databases

It takes more work to self-learn about database systems than it does with most other topics. It’s a relatively new (i.e. post 1970s) field of study with strong commercial incentives for ideas to stay behind closed doors. Additionally, many potentially excellent textbook authors have preferred to join or start companies instead.

Given the circumstances, we encourage self-learners to generally avoid textbooks and start with the [Spring 2015 recording of CS 186](https://archive.org/details/UCBerkeley_Course_Computer_Science_186), Joe Hellerstein’s databases course at Berkeley, and to progress to reading papers after.

One paper particularly worth mentioning for new students is “[Architecture of a Database System](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)”, which uniquely provides a high-level view of how relational database management systems (RDBMS) work. This will serve as a useful skeleton for further study.

_Readings in Database Systems_, better known as [the databases “Red Book”](http://www.redbook.io/), is a collection of papers compiled and edited by Peter Bailis, Joe Hellerstein and Michael Stonebraker. For those who have progressed beyond the level of the CS 186 content, the Red Book should be your next stop.

If you insist on using an introductory textbook, we suggest _[Database Management Systems](https://smile.amazon.com/Database-Management-Systems-Raghu-Ramakrishnan/dp/0072465638/)_ by Ramakrishnan and Gehrke. For more advanced students, Jim Gray’s classic _[Transaction Processing: Concepts and Techniques](https://www.amazon.com/Transaction-Processing-Concepts-Techniques-Management/dp/1558601902)_ is worthwhile, but we don’t encourage using this as a first resource.

It’s hard to consolidate databases theory without writing a good amount of code. CS 186 students add features to Spark, which is a reasonable project, but we suggest just writing a simple relational database management system from scratch. It will not be feature rich, of course, but even writing the most rudimentary version of every aspect of a typical RDBMS will be illuminating.

Finally, data modeling is a neglected and poorly taught aspect of working with databases. Our suggested book on the topic is _[Data and Reality: A Timeless Perspective on Perceiving and Managing Information in Our Imprecise World](https://www.amazon.com/Data-Reality-Perspective-Perceiving-Information/dp/1935504215)_.

### Languages and Compilers

Most programmers learn languages, whereas most computer scientists learn _about_ languages. This gives the computer scientist a distinct advantage over the programmer, even in the domain of programming! Their knowledge generalizes; they are able to understand the operation of a new language more deeply and quickly than those who have merely learned specific languages.

The canonical introductory text is _[Compilers: Principles, Techniques & Tools](https://smile.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811)_, commonly called “the Dragon Book”. Unfortunately, it’s not designed for self-study, but rather for instructors to pick out 1-2 semesters worth of topics for their courses. It’s almost essential then, that you cherry-pick the topics, ideally with the help of a mentor.

If you choose to use the Dragon Book for self-study, we recommend following a video lecture series for structure, then dipping into the Dragon Book as needed for more depth. Our recommended online course is [Alex Aiken’s, available from Stanford’s MOOC platform Lagunita](https://lagunita.stanford.edu/courses/Engineering/Compilers/Fall2014/about).

As a potential alternative to the Dragon Book we suggest _[Language Implementation Patterns](https://smile.amazon.com/Language-Implementation-Patterns-Domain-Specific-Programming/dp/193435645X/)_ by Terence Parr. It is written more directly for the practicing software engineer who intends to work on small language projects like DSLs, which may make it more practical for your purposes. Of course, it sacrifices some valuable theory to do so.

For project work, we suggest writing a compiler either for a simple teaching language like COOL, or for a subset of a language that interests you. Those who find such a project daunting could start with [Make a Lisp](https://github.com/kanaka/mal), which steps you through the project.

[![Compilers: Principles, Techniques & Tools](https://teachyourselfcs.com/dragon.jpg)](https://smile.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811) [![Language Implementation Patterns](https://teachyourselfcs.com/parr.jpg)](https://smile.amazon.com/Language-Implementation-Patterns-Domain-Specific-Programming/dp/193435645X/) 

> Don’t be a boilerplate programmer. Instead, build tools for users and other programmers. Take historical note of textile and steel industries: do you want to build machines and tools, or do you want to operate those machines?
>
>— Ras Bodik at the start of his compilers course

### Distributed Systems

As computers have increased in number, they have also _spread_. Whereas businesses would previously purchase larger and larger mainframes, it’s typical now for even very small applications to run across multiple machines. Distributed systems is the study of how to reason about the trade-offs involved in doing so, an increasingly important skill.

Our suggested textbook for self-study is Maarten van Steen and Andrew Tanenbaum’s _[Distributed Systems, 3rd Edition](https://www.distributed-systems.net/index.php/books/distributed-systems-3rd-edition-2017/)_. It’s a great improvement over the previous edition, and is available for free online thanks to the generosity of its authors. Given that the distributed systems is a rapidly changing field, no textbook will serve as a trail guide, but Maarten van Steen’s is the best overview we’ve seen of well-established foundations.

A good course for which some videos are online is [MIT’s 6.824](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB) (a graduate course), but unfortunately the audio quality in the recordings is poor, and it’s not clear if the recordings were authorized. *[Update @ Mar 2020: [the official lecture videos of the course](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB) has been published!]*

No matter the choice of textbook or other secondary resources, study of distributed systems absolutely mandates reading papers. A good list is [here](http://dsrg.pdos.csail.mit.edu/papers/), and we would highly encourage attending your local [Papers We Love](http://paperswelove.org/) chapter.

## Frequently asked questions

### What about AI/graphics/pet-topic-X?

We’ve tried to limit our list to computer science topics that we feel _every practicing software engineer_ should know, irrespective of specialty or industry. With this foundation, you’ll be in a much better position to pick up textbooks or papers and learn the core concepts without much guidance. Here are our suggested starting points for a couple of common “electives”:

*   For artificial intelligence: do [Berkeley’s intro to AI course](http://ai.berkeley.edu/) by watching the videos and completing the excellent Pacman projects. As a textbook, use Russell and Norvig’s _Artificial Intelligence: A Modern Approach_.
*   For machine learning: do Andrew Ng’s Coursera course. Be patient, and make sure you understand the fundamentals before racing off to shiny new topics like deep learning.
*   For computer graphics: work through [Berkeley’s CS 184](http://inst.eecs.berkeley.edu/~cs184/fa12/onlinelectures.html) material, and use [Computer Graphics: Principles and Practice](https://www.amazon.com/Computer-Graphics-Principles-Practice-3rd/dp/0321399528) as a textbook.

### How strict is the suggested sequencing?

Realistically, all of these subjects have a significant amount of overlap, and refer to one another cyclically. Take for instance the relationship between discrete math and algorithms: learning math first would help you analyze and understand your algorithms in greater depth, but learning algorithms first would provide greater motivation and context for discrete math. Ideally, you’d revisit both of these topics many times throughout your career.

As such, our suggested sequencing is mostly there to help you _just get started_… if you have a compelling reason to prefer a different sequence, then go for it. The most significant “pre-requisites” in our opinion are: computer architecture before operating systems or databases, and networking and operating systems before distributed systems.

### Who is the target audience for this guide?

We have in mind that you are a self-taught software engineer, bootcamp grad or precocious high school student, or a college student looking to supplement your formal education with some self-study. The question of when to embark upon this journey is an entirely personal one, but most people tend to benefit from having some professional experience before diving too deep into CS theory. For instance, we notice that students _love_ learning about database systems if they have already worked with databases professionally, or about computer networking if they’ve worked on a web project or two.

### How does this compare to Open Source Society or freeCodeCamp curricula?

The [OSS guide](https://github.com/open-source-society/computer-science) has too many subjects, suggests inferior resources for many of them, and provides no rationale or guidance around why or what aspects of particular courses are valuable. We strove to limit our list of courses to those which you _really should know_ as a software engineer, irrespective of your specialty, and to help you understand why each course is included.

freeCodeCamp is focused mostly on programming, not computer science. For why you might want to learn computer science, see [above](#why).

### What about language X?

Learning a particular programming language is on a totally different plane to learning about an area of computer science — learning a language is much _easier_ and much _less valuable_. If you already know a couple of languages, we strongly suggest simply following our guide and fitting language acquisition in the gaps, or leaving it for afterwards. If you’ve learned programming well (such as through _Structure and Interpretation of Computer Programs_), and especially if you have learned compilers, it should take you little more than a weekend to learn the essentials of a new language.

### What about trendy technology X?

No single technology is important enough that learning to use it should be a core part of your education. On the other hand, it’s great that you’re excited to learn about that thing. The trick is to work backwards from the particular technology to the underlying field or concept, and learn that in depth before seeing how your trendy technology fits into the bigger picture.

### Why are you still recommending the Dragon book?

The Dragon book is still the most complete single resource for compilers. It gets a bad rap, typically for overemphasizing certain topics that are less fashionable to cover in detail these days, such as parsing. The thing is, the book was never intended to be studied cover to cover, only to provide enough material for an instructor to put together a course. Similarly, a self-learner can choose their own adventure through the book, or better yet follow the suggestions that lecturers of public courses have made in their course outlines.

### How can I get textbooks cheaply?

Many of the textbooks we suggest are freely available online, thanks to the generosity of their authors. For those that aren’t, we suggest buying used copies of older editions. As a general rule, if there has been more than a couple of editions of a textbook, it’s quite likely that an older edition is perfectly adequate. It’s certainly unlikely that the newest version is 10x better than an older one, even if that’s what the price difference is!

### Who made this?

This guide was written by [Ozan Onay](https://twitter.com/oznova_) and [Myles Byrne](https://twitter.com/quackingduck), instructors at the [Bradfield School of Computer Science](https://bradfieldcs.com) in San Francisco. It is based on our experience teaching foundational computer science to hundreds of mostly self-taught engineers and bootcamp grads. Thank you to all of our students for your continued feedback on self-teaching resources. Thanks too to Alek Sharma, Omar Rayward, Ammar Mian and Tyler Bettilyon for feedback on this guide.

You may also like to join our mailing list:
