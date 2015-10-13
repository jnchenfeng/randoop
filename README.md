## What is Randoop? ##

Randoop is an automatic unit test generator for Java. It automatically creates unit tests for your classes, in JUnit format.

  * Randoop generates unit tests using feedback-directed random test generation. In a nutshell, this technique randomly, but smartly, generates sequences of methods and constructor invocations for the classes under test, and uses the sequences to create tests. Randoop executes the sequences it creates, using the results of the execution to create assertions that capture the behavior or your program and that catch bugs.
  * Randoop has created tests that find previously unknown errors even in widely-used libraries including Sun and IBM's JDKs. A .NET version of Randoop, used internally at Microsoft, has been used successfully by a team of test engineers to find errors in a core .NET component that has been heavily tested for years. Randoop's combination of randomized test generation and test execution results in a highly effective test generation technique.

### Randoop plugin for Eclipse ###

Check out the [Randoop plugin for Eclipse](https://rawgit.com/randoop/randoop/master/plugin/doc/index.html), which lets you automatically generate JUnit tests for your project.


---


## Documentation ##

[Randoop user manual](https://rawgit.com/randoop/randoop/master/doc/index.html)

[Randoop developer manual](https://rawgit.com/randoop/randoop/master/doc/dev.html)

[Project ideas page (for contributors/researchers)](https://github.com/randoop/randoop/wiki/ProjectIdeas)


---

### Randoop Publications ###

These papers describe Randoop and its underlying techniques in more detail.

[Eclat: Automatic generation and classification of test inputs](http://www.cs.washington.edu/homes/mernst/pubs/classify-tests-ecoop2005-abstract.html)
by Carlos Pacheco and Michael D. Ernst. In _ECOOP 2005 -- Object-Oriented Programming, 19th European Conference_, (Glasgow, Scotland), 2005.
Paper: [PDF](http://www.cs.washington.edu/homes/mernst/pubs/classify-tests-ecoop2005.pdf)

  * The first paper to present the feedback-directed random test generation, which generates each test, evaluates it, and determines whether to use it as a foundation for more tests.  Randoop uses this technique.

[Feedback-directed random test generation](http://www.cs.washington.edu/homes/mernst/pubs/feedback-testgen-icse2007-abstract.html)
by Carlos Pacheco, Shuvendu K. Lahiri, Michael D. Ernst, and Thomas Ball. In _ICSE '07: Proceedings of the 29th International Conference on Software Engineering_, (Minneapolis, MN, USA), 2007.
Paper: [PDF](http://homes.cs.washington.edu/~mernst/pubs/feedback-testgen-icse2007.pdf)
Slides: [PDF](http://homes.cs.washington.edu/~mernst/pubs/feedback-testgen-icse2007-slides.pdf) [PPT](http://homes.cs.washington.edu/~mernst/pubs/feedback-testgen-icse2007-slides.ppt)

  * The main paper describing feedback-directed random test generation and Randoop, as well as experiments that compare the technique with other test generation techniques.

[Randoop: Feedback-directed Random Testing for Java](http://people.csail.mit.edu/cpacheco/publications/randoop_for_java-abstract.html) by Carlos Pacheco and Michael D. Ernst. In _OOPSLA 2007 Companion_, Montreal, Canada, Oct. 2007, ACM.

  * A short tool paper describing aspects of the Java version of Randoop.

[Finding Errors in .NET with Feedback-directed Random Testing](http://people.csail.mit.edu/cpacheco/publications/randoop-case-study-abstract.html) by Carlos Pacheco, Shuvendu K. Lahiri, and Thomas Ball. In _ISSTA 2008_, Seattle, Washington, 2008.
Slides: [PPT](https://rawgit.com/randoop/randoop/master/presentations/issta_2008_final.pptx)

  * This case study details the use of Randoop at Microsoft (using a .NET version of Randoop, developed internally at Microsoft). A team of test engineers applied Randoop to a critical .NET component that had been thorughly tested for years. Still, Randoop found many serious errors.

Directed Random Testing (dissertation).
Slides: [PPT](https://rawgit.com/randoop/randoop/master/presentations/randoop2.ppt)


### Other publications that use or evaluate Randoop ###

Note: this list is seriously outdated!  For a more recent collection of publications take a look at [this Google Scholar search](http://scholar.google.com/scholar?hl=en&q=pacheco+lahiri+ball+ernst&btnG=Search&as_sdt=0%2C5&as_ylo=&as_vis=0).
There are 393 results as of 2015-05-10.

The following papers (by other authors) use or evaluate Randoop.

  * Predicting Effectiveness of Automatic Testing Tools by Brett Daniel and Marat Boshernitsan. In ASE 2008.
  * Predicting and Explaining Automatic Testing Tool Effectiveness by Brett Daniel and Marat Boshernitsan.UIUC Tech Report UIUCDCS-R-2008-2956.
  * Improving Structural Testing of Object-Oriented Programs via Integrating Evolutionary Testing and Symbolic Execution by Kobi Inkumsah and Tao Xie. In ASE 2008.
  * Making Program Refactoring Safer, by Gustavo Soares, Rohit Gheyi, Dalton Serey, and Tiago Massoni. In IEEE Software, July/August 2010.

### Courses that use Randoop ###

Note: this list is seriously outdated!
If you wish to have your course listed here, let us know.

  * Software Testing (Spring 2008) at Universidade Federal de Pernambuco, taught by Marcelo d'Amorim.
  * Reliable Software: Testing and Monitoring (Third term 2008), Caltech, taught by Alex Groce.
  * UIUC Topics in Software Engineering (Randoop was used in this course in [Fall 2007](https://agora.cs.illinois.edu/display/cs527/Home), [Fall 2008](https://agora.cs.illinois.edu/display/cs527fa08/Home), and [Fall 2010](https://agora.cs.illinois.edu/display/cs527fa10/Home).
  * Automatic Program Checking, Karlsruhe Institute of Technology (2010).
  * RIO 2011 C5: Automated Test Generation and Repair.
  * Automatic Program Checking, Karlsruhe Institute of Technoloy (2010, 2011)




### .NET version of Randoop ###

A version of Randoop that works with Microsoft's .NET platform is available at [http://randoop.codeplex.com/](http://randoop.codeplex.com/).  Check it out!  Randoop.NET is a from-scratch re-implementation of feedback-directed test generation.  Also, the "Randoop" name is due to the Microsoft group, even though the idea and the Java tool (previously known as "Joe") predate their work.  The project was created in September 2010, but no further development was done.  (The [discussions webpage](http://randoop.codeplex.com/discussions) has only two conversations, both from 2011.)
