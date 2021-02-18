# CourseGraphDB
in this folder you will find graph database example of a our ITPH course.
after creation you can run one of the quieres: 

q1: people who owns certification of AZ900 with thier marks
g.V('az.900').inE('owns').as('a').outV().as('b').select('a','b').by('mark').by('fname')
q2: how many courses does stef organise
g.V('stef.1').outE('organise').count()
q3: name of the students that remsey teachs.
g.V('remsey.1').out('teaches').in('enroll').values('fname','lname')

try more ......
