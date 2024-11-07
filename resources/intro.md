## 编译器简介

**编译器**（compiler）是一种电脑程序，它会将某种程序语言写成的原始码（原始语言）转换成另一种程序语言（目标语言，通常具有称为目标代码或机器代码的二进制形式）。[这里](https://www.bilibili.com/video/BV1hDH6e2E1N/?spm_id_from=333.999.0.0&vd_source=398e568c91ee314006233fcd3b521042)有一份关于编译器原理的趣味性介绍。

编译器主要的目的是将便于人编写、阅读、维护的高级计算机语言所写作的原始码程序，翻译为计算机能解读、运行的低阶机器语言的程序，也就是执行文件。编译器将原始程序（source program）作为输入，翻译产生使用目标语言（target language）的等价程序。源代码一般为高阶语言（High-level language），如Pascal、C、C++、C# 、Java等，而目标语言则是汇编语言或目标机器的目标代码（Object code），有时也称作机器代码（Machine code）。

一个现代编译器的主要工作流程如下：

源代码（source code）→ 预处理器（preprocessor）→ 编译器（compiler）→ 汇编程序（assembler）→ 目标代码（object code）→ 链接器（linker）→ 执行文件（executables），最后打包好的文件就可以给电脑去判断执行了。

早期的计算机软件都是用汇编语言直接编写的，这种状况持续了数年。当人们发现为不同类型的中央处理器（CPU）编写可重用软件的开销要明显高于编写编译器时，人们发明了高级编程语言。由于早期的计算机的内存很少，当大家实现编译器时，遇到了许多技术难题。

大约在20世纪50年代末期，与机器无关的编程语言被首次提出。随后，人们开发了几种实验性质的编译器。第一个编译器是由美国女性电脑科学家葛丽丝·霍普（Grace Murray Hopper）于1952年为A-0 系统编写的。但是1957年由任职于IBM的美国电脑科学家约翰·巴科斯（John Warner Backus）领导的FORTRAN则是第一个被实作出具备完整功能的编译器。1960年，COBOL成为一种较早的能在多种架构下被编译的语言。

高级语言在许多领域流行起来。由于新的编程语言支持的功能越来越多，计算机的架构越来越复杂，这使得编译器也越来越复杂。

早期的编译器是用汇编语言编写的。首个能编译自己源程序的编译器是在1962年由麻省理工学院的Hart和Levin制作的。从20世纪70年代起，实现能编译自己源程序的编译器变得越来越可行，不过还是用Pascal和C语言来实现编译器更加流行。制作某种语言的第一个能编译器，要么需要用其它语言来编写，要么就像Hart和Levin制作Lisp编译器那样，用解释器来运行编译器。

20 世纪 70 年代末，Production Quality Compiler-Compiler 项目引入了至今仍广泛使用的编译器组织原则（例如，前端处理语法和语义以及后端生成机器代码）。

### 早期编译器

早期计算机的软件主要是用汇编语言编写的，在此之前直接用机器代码编写。对于程序员来说，使用高级语言通常会更有效率，并且用高级语言编写的程序可以在不同类型的计算机上重用。即便如此，编译器的建立还是花了一段时间，因为它们生成的代码性能不如手写的汇编程序，它们本身的开发项目令人畏惧，而且早期计算机非常有限的内存容量导致了许多错误。实际编译器实现的技术问题。

1942 年至 1945 年间，Konrad Zuse 开发了 Plankalkül（“计划演算”），这是第一种计算机高级语言，他为此设想了一个 Planfertigungsgerät（“计划汇编设备”），它可以自动翻译程序的数学公式转化为机器可读的打孔胶片。然而，该语言的第一个实际编译器仅在几十年后才实现。

1949 年至 1951 年间，Heinz Rutishauser 提出了 Superplan，一种高级语言和自动翻译器。他的想法后来被 Friedrich L. Bauer 和 Klaus Samelson 完善。

第一个实用编译器是 Corrado Böhm 于 1951 年为他的博士论文编写的，这是世界上第一批授予计算机科学博士学位的论文之一。

第一个实现的编译器是由 Grace Hopper 编写的，她还创造了术语“编译器”，指的是她的 A-0 系统，该系统充当加载器或链接器，而不是现代概念的编译器。现代意义上的第一个自动编码和编译器是由 Alick Glennie 于 1952 年在曼彻斯特大学为 Mark 1 计算机开发的。IBM 的 John W. Backus 领导的 FORTRAN 团队于 1957 年推出了第一个商用编译器，花费了 18 个人年的时间才创建出来。

第一个 ALGOL 58 编译器于 1958 年底由 Friedrich L. Bauer、Hermann Bottenbruch、Heinz Rutishauser 和 Klaus Samelson 为 Z22 计算机完成。鲍尔等人。前几年一直致力于 Sequentielle Formelübersetzung（即顺序公式翻译）的编译器技术。

到 1960 年，Philco 2000 上提供了扩展的 Fortran 编译器 ALTAC，因此很可能在 1960 年中期为 IBM 和 Philco 计算机架构编译了 Fortran 程序。 [11]第一个已知的演示跨平台高级语言是 COBOL。在 1960 年 12 月的演示中，在 UNIVAC II 和 RCA 501 上编译并执行了 COBOL 程序。


## 参考文献

1. Chakraborty, P., Saxena, P. C., Katti, C. P., Pahwa, G., Taneja, S. A new practicum in compiler construction. _Computer Applications in Engineering Education_ , In Press. [链接](http://onlinelibrary.wiley.com/doi/10.1002/cae.20566/pdf) （页面存档备份，存于互联网档案馆）
2. [The ACM Digital Library](https://web.archive.org/web/20070717153035/http://www.acm.org/classics/dec95/). （原始内容存档于2007-07-17）.

* 本文档来自[维基百科](https://zh.wikipedia.org/wiki/%E7%B7%A8%E8%AD%AF%E5%99%A8#cite_ref-1)，更详细的编译器发展历史可以阅读[这里](https://en.wikipedia.org/wiki/History_of_compiler_construction)。

## 延伸阅读

- LLVM community. [The LLVM Target-Independent Code Generator](https://web.archive.org/web/20210501144108/http://llvm.org/docs/CodeGenerator.html#built-in-register-allocators). LLVM Documentation.  [17 June 2016]. （原始内容存档于2021-05-01）.
- [Compiler textbook references](https://web.archive.org/web/20150103161301/http://www.informatik.uni-trier.de/~ley/db/books/compiler/index.html) A collection of references to mainstream Compiler Construction Textbooks
- [Aho, Alfred V.](https://en.wikipedia.org/wiki/Alfred_V._Aho); [Sethi, Ravi](https://en.wikipedia.org/wiki/Ravi_Sethi); [Ullman, Jeffrey D.](https://en.wikipedia.org/wiki/Jeffrey_D._Ullman) Compilers: Principles, Techniques, and Tools 1st. [Addison-Wesley](https://en.wikipedia.org/wiki/Addison-Wesley). 1986. ISBN 9780201100884.
- [Allen, Frances E.](https://archive.org/details/sim_ibm-journal-of-research-and-development_1981-09_25_5/page/535) A History of Language Processor Technology in IBM. IBM Journal of Research and Development (IBM). September 1981, **25** (5): 535–548. [doi:10.1147/rd.255.0535](https://dx.doi.org/10.1147%2Frd.255.0535).
- [Appel, Andrew Wilson](https://en.wikipedia.org/wiki/Andrew_W._Appel). Modern Compiler Implementation in Java 2nd. [Cambridge University Press](https://en.wikipedia.org/wiki/Cambridge_University_Press). 2002. ISBN 978-0-521-82060-8.
- [Appel, Andrew Wilson](https://en.wikipedia.org/wiki/Andrew_W._Appel). [Modern Compiler Implementation in ML](https://web.archive.org/web/20210427035906/https://books.google.com/books?id=8APOYafUt-oC). [Cambridge University Press](https://en.wikipedia.org/wiki/Cambridge_University_Press). 1998  [2020-01-11]. ISBN 978-0-521-58274-2. （原始内容存档于2021-04-27）.
- [Bornat, Richard](https://en.wikipedia.org/wiki/Richard_Bornat). [Understanding and Writing Compilers: A Do It Yourself Guide](https://web.archive.org/web/20070615132948/http://www.cs.mdx.ac.uk/staffpages/r_bornat/books/compiling.pdf) (PDF). [Macmillan Publishing](https://en.wikipedia.org/wiki/Macmillan_Publishers). 1979  [2020-01-11]. ISBN 978-0-333-21732-0. （原始内容 (PDF)存档于2007-06-15）.
- Cooper, Keith Daniel; Torczon, Linda. [Engineering a compiler](https://archive.org/details/engineeringcompi00coop_143) 2nd. Amsterdam: Elsevier/Morgan Kaufmann. 2012: [8](https://archive.org/details/engineeringcompi00coop_143/page/n32). ISBN 9780120884780. OCLC 714113472.
- [McKeeman, William Marshall](https://en.wikipedia.org/wiki/William_M._McKeeman); [Horning, James J.](https://en.wikipedia.org/wiki/Jim_Horning); Wortman, David B. [A Compiler Generator](https://archive.org/details/compilergenerato00mcke). [Englewood Cliffs, NJ](https://en.wikipedia.org/wiki/Englewood_Cliffs,_NJ): [Prentice-Hall](https://en.wikipedia.org/wiki/Prentice-Hall). 1970. ISBN 978-0-13-155077-3.
- [Muchnick, Steven](https://en.wikipedia.org/wiki/Steven_S._Muchnick). [Advanced Compiler Design and Implementation](https://web.archive.org/web/20210223022312/https://books.google.com/books?id=Pq7pHwG1_OkC). [Morgan Kaufmann Publishers](https://en.wikipedia.org/wiki/Morgan_Kaufmann_Publishers). 1997  [2020-01-11]. ISBN 978-1-55860-320-2. （原始内容存档于2021-02-23）.
- [Scott, Michael Lee](https://en.wikipedia.org/wiki/Michael_L._Scott). [Programming Language Pragmatics](https://web.archive.org/web/20210427012533/https://books.google.com/books?id=4LMtA2wOsPcC) 2nd. [Morgan Kaufmann](https://en.wikipedia.org/wiki/Morgan_Kaufmann). 2005  [2020-01-11]. ISBN 978-0-12-633951-2. （原始内容存档于2021-04-27）.
- Srikant, Y. N.; Shankar, Priti. [The Compiler Design Handbook: Optimizations and Machine Code Generation](https://web.archive.org/web/20210427020439/https://books.google.com/books?id=0K_jIsgyNpoC). [CRC Press](https://en.wikipedia.org/wiki/CRC_Press). 2003  [2020-01-11]. ISBN 978-0-8493-1240-3. （原始内容存档于2021-04-27）.
- Terry, Patrick D. [Compilers and Compiler Generators: An Introduction with C++](https://web.archive.org/web/20150914062457/http://www.scifac.ru.ac.za/compilers/conts.htm). International Thomson Computer Press. 1997  [2020-01-11]. ISBN 978-1-85032-298-6. （原始内容存档于2015-09-14）.
- [Wirth, Niklaus](https://en.wikipedia.org/wiki/Niklaus_Wirth). [Compiler Construction](https://web.archive.org/web/20170217071020/http://www.ethoberon.ethz.ch/WirthPubl/CBEAll.pdf) (PDF). [Addison-Wesley](https://en.wikipedia.org/wiki/Addison-Wesley). 1996  [2020-01-11]. ISBN 978-0-201-40353-4. （原始内容 (PDF)存档于2017-02-17）.
