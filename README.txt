Introduction to Computer Graphics CS 174A: Assignment 1
Weight: 15 %
Points: 24
Collaboration: None permitted. If you discuss this assignment with others you should submit
their names along with the assignment material.
Reverse engineering the sample executable and using code from previous offerings of the course
constitute plagiarism and are strictly prohibited. We will use automated tools to check for plagiarism.
Submission: Follow the instructions carefully to avoid point reductions.
Submit via CourseWeb a zipped file including a Visual Studio 2008 or 2010 project directory
with project files. Remove the executable and object files (you can use Clean Project in the
Debug menu). Include ALL the code necessary to compile and run your project.
Your project must compile and run on SEAS lab machines.
Write a program in OpengGL that draws the scene shown in the sample executable. Use the template
code in template3.zip, which is provided on the course website. For drawing objects, use
only the procedures provided, drawCube() and drawSphere(); do NOT use glutSolidSphere() or
glutSolidCube() or any other built-in cube and sphere drawing functions. You may use OpenGL
functions such as glTranslatef(), glRotatef(), glScalef(), glPushMatrix(), and glPopMatrix().
Requirements:
(a) You must use a hierarchical approach to model the complex objects. (5 Points)
(b) Model a static ground plane. (1 Point)
(c) Model a tree that has a trunk made of 8 parts and a sphere for foliage. (2 Points)
(d) The tree must visibly sway as shown by the sample executable. (2 Points)
(e) You must rotate objects around the correct point; i.e., where they touch the parent object.
Trunk parts rotate around the middle of the bottom face. (4 Points)
(f) Animate the wings and legs of the wasp. You may use the same value for more than one
angle. The wasp’s main axis is X. All moving body parts must rotate around the X-axis.
(5 Points)
(g) The wasp flies in a circle around the vertical axis, and it should always be aligned with
the tangent of the circle. (3 Points)
(h) The wasp must move up and down. (2 Points)
(i) You need NOT match the exact motion or dimensions of the sample code; however, your
scene must be qualitatively and visually similar to the one provided.
Hints:
(a) Create a function drawLeg() and use it for all the legs.
(b) Call your drawing function in display(). Use the TIME variable.
(c) Functions of the form f(t) = a + b*sin(w*t) are useful for modeling periodic motion.