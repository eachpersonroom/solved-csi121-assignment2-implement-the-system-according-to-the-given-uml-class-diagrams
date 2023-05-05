Download Link: https://assignmentchef.com/product/solved-csi121-assignment2-implement-the-system-according-to-the-given-uml-class-diagrams
<br>
This assignment requires you to write a program in Java that help two students to enrol into the Bachelor of Computer Science course and the Master of Computer Science course, respectively. You will be asked to use the OOP concepts such as the inheritance, polymorphism, abstract class/method, and interface to implement the program.

<strong> </strong>Background

Assignment 2 is based on the Assignment 1 (please see Moodle for Assignment 1’s solution). Please refer to Assignment 1’s description for the Bachelor of Computer Science course structure. In Assignment 2, the Master of Computer Science course will be added.

The Master of Compute Science course contains three parts, i.e., the core subjects, the majors and the elective subjects. In order to complete the course, students shall complete at least 96 credit points.

<ol>

 <li>All students shall complete 8 core subjects, i.e., 54cp in total.</li>

 <li>All students shall complete a major with three subjects, i.e., 18cp in total. The course contains four majors and each student can only select one major. The four majors are Intelligent Systems, Machine Learning and Big Data, Network and Information Security, and Software Engineering. The core subjects of each major are displayed in the following snapshots</li>

 <li>All students shall enrol 4 elective subjects to make up 96 credit points. (Students are allowed to enrol more than 96 credit points). The elective subjects are the collection of subjects from all four major cores plus the following six subjects.</li>

 <li>You are required to design, implement and test a student system to enrol two students into the Bachelor of Computer Science course and the Master of Computer Science, respectively. The UML class diagram of the system is given as below. You can add new classes, or fields and methods for the existing classes, but <strong><u>can’t</u></strong> delete any existing classes, fields or methods (The .uxf file of the class diagram is also provided. The .uxf file can be opened by Umlet and you can modify the class diagram based on your new design).</li>

</ol>




<ol start="5">

 <li>The StudentSystem class (primary class)</li>

</ol>

The StudentSystem class is the primary class and contains the main() method and a static students field. In Assignment 2, the following steps shall be competed inside the main() method. Please note the following steps shall be conducted consequentially without re-running the program.

<ol>

 <li>to create all subjects, majors, and courses based on the Bachelor of Computer Science (see Assignment 1 description for BCS hardcode) and the Master of Computer Science structures. You can use the following hardcore or your own way to create the subject, major and course objects;</li>

 <li>to enrol the first student to the Bachelor of Computer Science course. The program shall display the BCS structure first and ask the user to input the first student’s information (see the below example for details). Then the system will create the first student object (declared with the Student class and created with Undergraduate class constructor). The system will automatically enrol the student to all BCS core subjects and ask the student to select a major and several elective subjects to complete the enrolment. This procedure is same as what you did in Assignment 1. However, in Assignment 2, a Record object shall be created first based on the first student’s enrolment information, then the Record object shall be added to the first student’s records list.</li>

</ol>

<ul>

 <li>to enrol the second student to the Master of Computer Science course. It is assumed that the second student already completed his/her Bachelor of Computer Science course with the exact same subjects as the first student. Therefore, a clone of the first student’s BCS record will be created and added to the second student’s enrolment record first automatically. Then the system will enrol the second student to the Master of Computer Science course. The detailed steps are:

  <ol>

   <li>to displayer the welcome information for the second student and display the Master of</li>

  </ol></li>

</ul>

Computer Science course structure to the second student;

<ol>

 <li>to create the second student object (declared with Student class and created with</li>

</ol>

Postgraduate class constructor) and ask the second student input some personal details.

Very similar as the information provided by the first student, but the second student needs to provide the completion session and year for this/her bachelor degree;

<ol>

 <li>to create a clone object (deep clone) of the first student’s BCS record, modify the clone object’s status to COMPLETE, and add the clone object to the second student’s enrolment record list;</li>

 <li>to automatically enrol the second student to all core subjects of MCS, and ask the second student to select a major and 4 elective subjects to complete the enrolment. The second student’s enrolment record of MCS shall be kept by another Record object (the status shall be ACTIVE). The second Record object shall be added to the second student’s records list finally;</li>

 <li>to add the Undergraduate student and the Postgraduate student objects to the static students</li>

</ol>

ArrayList;

<ol>

 <li>to use a for loop to display all students’ enrolment information in the students ArrayList. For each student, you shall display the student’s personal information first, and then all enrolment records of the student. The Undergraduate student shall have one enrolment record and the Postgraduate student shall have two enrolment records.</li>

 <li>to use the “instanceof” and “down casting” in the for loop above to show the bachelor completion time for the Postgraduate student (calling the specific getBachelorCompletion() method defined in the Postgraduate class).</li>

</ol>










See the snapshots of an example for the program testing. Your program must have the exact same outputs for the same inputs. The user’s inputs are highlighted by blue colour. The watermark is used to prevent my snapshots are used in your reports. You must capture the snapshots of your own program’s outputs and compilation.







<strong>(Enrol the first student to the Bachelor of Computer Science course) </strong>

<strong>Welcome to enrol the Bachelor of Computer Science course. The course structure is as follows: </strong>

<strong>Cores:  </strong>

<strong>Electives:  </strong>

<strong>Electives: </strong>

<strong>  record.) </strong>

<strong>Cores:  </strong>

<strong>Electives:  </strong>




<strong>Electives: </strong>

<strong>Cores:  </strong>

<strong> </strong>

<strong>Electives:  </strong>

<strong>Cores:  </strong>

<strong>Electives:  </strong>

<strong> </strong>

<strong>Cores:  </strong>




<strong>Electives:  </strong>

<strong> </strong>Tasks

Task 1 : Implement the system according to the given UML class diagrams. If you add new classes, fields or methods in the UML class diagrams, please also include the new diagram in your submission. The program shall

<ul>

 <li>be consistent with the UML class diagrams;</li>

 <li>follow the conventions for naming all classes, variables, and methods;</li>

 <li>provide sufficient comments;</li>

 <li>use proper blank spaces, indentation and braces to make your code easy to read and understand;</li>

 <li>follow the steps specified in StudentSystem class to enrol two students into the Bachelor of Computer Science course and Master of Computer Science course, respectively;</li>

 <li>be able to automatically calculate the remaining elective subject number for the minimal credit points requirement;</li>

 <li>implement the Cloneable (deep clone) and Enrolment interface;</li>

 <li>implement abstract super class and abstract methods;</li>

 <li>override abstract methods in sub class with polymorphism;</li>

 <li>use the instanceof and down casting to cast a super class object to a sub class object for calling the specific methods defined in the sub class.</li>

</ul>

Task 2: Compilation and test. You should compile and test your program by using two different cases. The first testing case must use the exact same inputs in the given example. The second testing case must choose different majors and elective subjects for the two students. Please carefully compile and test your program and make sure your program can pass the compilation by using “javac” command. Please do not define the package in your program (a special alert for students who use IDE to complete the assignment).