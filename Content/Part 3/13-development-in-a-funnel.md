## 13. Development in a Funnel

Following the release of WordPress 1.5, software development process changed. This was precipitated by a shift in the version control system [from CVS to a more modern version control system, Subversion (SVN)](http://lists.wordpress.org/pipermail/hackers/2005-February/004078.html)[^fn-1]. The most active contributors at that time were Ryan and Matt, so when the move was made none of the other original developers had their commit access renewed.

This started a long period in which WordPress development operated through a funnel. Contributors created a patch, upload it to mosquito (and later trac) [^fn-2], it was reviewed by one of the committers who committed the code to the main repository. Over time, the funnel became smaller as Matt’s focus went elsewhere and development was driven by Ryan. This style of development has its advantages and disadvantages, and it was frequently the subject of discussion amongst the community, particularly on wp-hackers. The advantage of a funnelling process is that disagreements about code happen on the mailing list, before a change lands in the repository. The disadvantage is that one person has to review every patch, which frustrates the developers waiting for their patches to be committed. 

This approach to development was heavily influenced by the Linux project, which Ryan had some involvement with in the past. As WordPress began to really take shape as recognizable Free Software project, with a defined development process and proper developer infrastructure, many of these changes were guided by Ryan’s previous experience. WordPress did differ in the fact that [Linux has only one committer](http://www.linuxfoundation.org/content/23-how-patches-get-kernel) - the project founder Linus Torvalds - whereas WordPress had two. Over the years this opened up to more and more committers. The other difference is that Linux has a number of maintainers who maintain different subsystems before pushing patches upstream. This means that Torvalds doesn’t review all of the thousands of patches that go into the kernel. He just reviews a fraction of them and review is delegated to trusted subsystem maintainers. Although WordPress in the future would move towards component maintainers, it never followed Linux in this manner.


 A committer is someone who can use the commit command to make changes to the group’s central repository. The number of people who can do this on a project varies, with projects deciding on the number of committers depending on their own structure and philosophies. The question of who should have commit access to the WordPress repository comes up again and again. There are regular threads requesting that more people be given commit. 

There are a number of reasons that people request commit access: to speed up the development process, to prevent situations in which patches wait months for a review, to acknowledge the contributions of project regulars, to create a more egalitarian project structure. Adding a new committer to a project is a major decision and the project’s approach changed dramatically from the wild west days of coding in WordPress 0.7. As the project got on its feet, anyone who demonstrated some technical expertise and a small amount of dedication was given commit access. All of those developers could commit code to the repository whenever they wanted. But as the project grew, and the number of users grew, it became more important to have some sort of filtering mechanism. A committer is the filter through which the code is passed. When someone is given commit access to the repository it demonstrates a level of trust. It signifies that a contributor is trusted enough to know which code should make it in to WordPress.

[Karl Fogel describes committers as](http://producingoss.com/en/producingoss.html#committers) “the only formally distinct class of people found in all open source projects.”  “Committers are an unavoidable concession to discrimination in a system which is otherwise as non-discriminatory as possible,” he writes. As much as one tries to maintain that commit is a functional role, commit access is a symbol of trust, both in terms of coding skills and in terms a person’s adherence to the project’s core beliefs and ethos. It creates a power dynamic between those that have commit access and those that don’t.

The role of a committer is to provide quality control. To decide who to give commit access to, a project maintainer has to first find people who not only write good code but who are good at reviewing other people’s code. This means being good at recognising places in which code can be improved and being constructive when providing feedback. But there are other, social skills that go along with being a committer. For one, the person needs to demonstrate an adherence to a project’s ideals. In the case of WordPress, this means being fully committed to the project’s user-first approach. Another skill they need to have is to be able to “[play well in the sandbox](http://producingoss.com/en/committers.html#choosing-committers)”. Someone may write flawless code, but if they are unable to work with others they aren’t going to make a wonderful committers. It’s important to make good choices about who is given commit access because once it has been given to someone it is difficult to take it away.

In an attempt to avoid an “us and them” mentality in which committers have a higher status than everyone else, the WordPress project had only two committers. This meant that everyone was subject to the same review process and the same rules. Opening it up to more people may create a feeling of dissatisfaction amongst those who don’t have commit access. But by not opening it up at all, there was a sense of frustration amongst developers who felt that they could never progress within the current project structure. The other disadvantage to having so few committers is that in a growing project with patches mounting there weren’t enough resources to review all of the patches and many of them languished on trac. 

There is a perennial tug of war between those who contribute to the project and those who maintain it, and even amongst the project leaders themselves. Who gets commit access? How long for? What sort of status is attached to commit? Should only lead developers be committers? What is a lead developer anyway? Over the coming years these questions were played out at various stages of the project’s development. 


[^fn-1] A version control system is a tool for managing the changes to a piece of software, document, or other collection of information. Each change is identified by a number and the name of the person who has made the change. They are often accompanied by comments about what that change is. A version control system allows a project to keep track of changes and also to revert changes as necessary.

[^fn-2] The first bug tracker used by the WordPress project was mosquito. Later bug tracking with moved to Trac.