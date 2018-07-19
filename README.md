# EducationalTools
all tools working for Education
I also add all related resources here

https://github.com/PomonaSakai/EducationalTools/tree/master



#####
##### github classroom with LTI  (2016/Oct)
from https://education.github.community/t/how-do-students-submit-their-assignments/3196/14
Hi, I work in the Academic Apps group (we manage the web apps like Bb Learn, etc) at a university and was looking for the LTI setup instructions for Classroom, and I think I’ve realized that there aren’t any because Classroom doesn’t have LTI support…

    So no one has to go look it up, LTI = Learning Tools Interoperability 3, it’s basically OAuth2 for LMS platforms to communicate with gradable external tools without having to code platform specific integrations - in short, LTI makes any gradable web tool integrated with Blackboard Learn, Instructure Canvas, Sakai, Moodle, etc.

If enabled, the workflow @gcschmit describes above would be automated to a larger degree - based on some unfinished LTI hacking 3 I’ve done, it could look like this:

    Instructor pastes an LTI-invitation link into their blackboard/canvas/etc (LMS) class
    Instructor follows the link and selects/creates the github classroom assignment
    Student follows the link and classroom receives info that links back to the LMS (student identifier, course identifier, assignment identifier) - as a bonus github would automatically receive all the information needed for the student to create an account, so it would be much like logging in to another webapp via github (or facebook, etc.), i.e. a frictionless account creation
    Student does the assignment
    If there is a way for instructors to grade assignments (I couldn’t find one), the grade could be passed back to the LMS (a feature I can assure you that instructors love)
So what would be the best way to encourage LTI support from github’s side? Our school has very heavy LMS usage (usually above 90% of undergrad courses use it (~4,900 this semester), to the point where a lot of our support in the Fall is explaining to students that a course doesn’t’ necessarily have to use blackboard, we don’t actually require it of instructors), and so any tool that we suggest usually has some form of LTI support, mainly because of how much it automates in terms of assessment.

### github in Canvas
from https://community.canvaslms.com/thread/7640
So to recap, my suggestion if you want nice looking pages displayed in your iframe, use Github Pages.
1. Go to https://pages.github.com
2.  Click "Project Site"
3. Follow the instructions there to create your gh-pages branch and create your first page
4. Embed your new Github pages page into your Canvas content page using an iframe with code something like:
    <iframe src="https://musebrarian.github.io/<project-name>/<page-name>" width="100%" height="600"></iframe>  
Now you can use all the Github power of version control on those pages plus have them embedded into your Canvas course and have them update in Canvas when you change them in Github.
