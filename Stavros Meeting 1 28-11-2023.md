tavros notes

A USER WILL OPERATE THE SOFTWARE


-- Lecturer name
-- Module title
-- Module reference (eee_5...)
-- Module type (lecture, workshop, tutorial)
--Class groups (5607, 5604, both are different but might belong to one classroom/lecture)
-- Classroom (have database), [classroom size, have columns for lab rooms, lectures rooms, etc  ]
-- Should be able to add or remove things from database


DATABASE:
classrooms, lecturers, module (in courses)
+
ensure no big time gaps (of like 5 hours), the room stays the same, smooth timetable, lunch breaks, restrictions (no midnight and stuff like that)
+
"I want to exclude wednesday from 1 to 5pm" -> create fake timeslot that triggers timeclash algorithm to prevent timeslots in those times


include some automation meaning include a default setting? (automatic or manual mode)

MONDAY 9 AM TO FRIDAY 5 PM


implement this in the algorithm:
consider full time students (9 am to  9 pm) - MULTIPLE DAYS [3]
and part time students (9 am to 5 pm) - ONLY ONE DAY
there should be an error if this is broken

ensure that multiple years of one course do not have the same days across their timetables

eg. year 1monday
year 2 tuesday
year 3 thursday
year 4 friday(?)

postgraduate -> wednesday


i want to search by module, give me all of those.

THIS COUNTS AS A SGR1 meeting

this one is basically nov/december
next: 1 in january, 1 in feb, 1 in march

options for meeting dates
tuesday 11-12 (just before 12)
thursday before 2pm