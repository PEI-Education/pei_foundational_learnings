# pei_foundational_learnings
PowerSchool customization for tracking PEI's Foundational Learnings

## Features
**PowerTeacher**: 
*Student Profile*:
- A page in /studentpages/ for each grade level from K-9 with appropriate FLs.
- Run Special Operation > Rebuild Custom Page Links to make "Foundational Learnings" appear in Backpack nav menu and default page dropdown in "Manage Profile"
- Initial foundational_learnings page redirects to appropriate grade_level for studentpages
- Once an FL is marked Y or Y*, can no longer be edited from teacher interface
- Teacher can only add comment, name, school and year on the page for the student's current grade level.

*Class Profile*:
- Linked from left sidebar on student info pages.
- Provide a view of FL status for all students in a section.
- Broken down by subject, and into manageable chunks by putting K-3, 4-6, and 7-9 on separate tabs.
- Printable: Using the Print Report button the upper right, only table will print (normal print leaves some PS header info)
  
**PowerSchool SIS**: Same page layout as on PowerTeacher, but any FL can be modified at any time. Profile reports are linke from main tab on System Reports page.

## Version/Release Notes
  - **0.9.6**: Added Math, ELA and FLA Profiles to Admin.
  - **0.9.5**: Added Mathematics, ELA and FLA Class Profiles to PowerTeacher, with sticky header, highlighting of N, and links back to students' individual profiles for easy access to comments.
  - **0.9.0**: Added ELA Writing FLs to Grades 7 and 8.
  - **0.8.0**: Fixed textarea tags to handle line-breaks properly.
  - **0.7.2**: Hid FLs for 7-9 FLA.
  - **0.7.1**: Exposed FLs for 1-6 FLAs in the teacher interface.
  - **0.7.0**: Cleanup of schema and pages for FLA FLs in prep for French data import.
  - **0.6.0**: Removed limitations on access on SIS; rebuilding custom links for PT.
  - **0.5.0**: Initial launch version for production - no 7-9 FLA outcomes, no links to interface for most users (initialLaunch branch)
  - **0.4.1**: Minor fixes to schema and bug fixes
  - **0.4.0**: Fixed FL numbering on Grades 7-9; added admin pages.
  - **0.3.3**: Removed old FI outcomes from pages and DB schema; added test admin page; implemented all coach feedback on PowerTeacher pages.
