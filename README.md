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

## Note on Field Name/Label Alignment

In fall 2024, English Programs requested we re-number many of the Foundational Learnings for math. This work was completed in the front end, but the back end was not updated. The field names in the database are still the old numbers, but the labels on the front end are the new numbers. This is not a problem for the user, but it is important to note for anyone writing a query. The file PowerSchool Changes.xlsx in the root of this repository has a list of the old and new numbers for reference.

## Version/Release Notes

- **2025.5.3**: Fixed alignment of grade level headers to outcomes in Class Profile reports.
- **2025.5.2**: Removed Grade 1 ELA RS1, RS2.
- **2025.5.0**: Added requested edits to Math numbering after testing.
- **2024.12.1**: Updated Math FL numbering to match new curriculum guides. See note above on field-name/label alignment.
- **2024.12.0**: Removed school and year dropdown selectors from printouts of class profile reports for admins.
- **2024.4.3**: Added Writing School-Based Assessment for Grade 4.
- **2024.4.2**: Added Class Profiles compatibility with EUI.
- **2024.4**: Added Math School-Based Assessment for Grade 3 and minimal EUI support.
New numbering scheme above this point.
- **1.0.1**: Updated tab IDs for printing.
- **1.0**: Fixed runreports page fragment issue. Ready to install on production.
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
