# HackerRank_SQL-test
SELECT a.roll_number, a.name
from student_information as a
INNER JOIN examination_marks as b
ON a.roll_number = b.roll_number
GROUP by a.roll_number
HAVING SUM(b.subject_one + b.subject_two + b.subject_three) < 100;
