# pei_foundational_learnings
PowerSchool customization for tracking PEI's Foundational Learnings

## Features
**PowerTeacher**: A page in /studentpages/ for each grade level from K-9 with appropriate FLs.
- Run Special Operation > Rebuild Custom Page Links to make "Foundational Learnings" appear in Backpack nav menu and default page dropdown in "Manage Profile"
- Initial foundational_learnings page redirects to appropriate grade_level for studentpages
- Once an FL is marked Y or Y*, can no longer be edited from teacher interface
- Teacher can only add comment, name, school and year on the page for the student's current grade level.

**PowerSchool SIS**: Same page layout as on PowerTeacher, but any FL can be modified at any time.

## Version/Release Notes
**0.4.0**: Fixed FL numbering on Grades 7-9; added admin pages.
**0.3.3**: Removed old FI outcomes from pages and DB schema; added test admin page; implemented all coach feedback on PowerTeacher pages.
