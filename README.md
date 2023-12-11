# Digital Tutoring Platform as a Service
<p style="text-align: center;">SE 673 | Project Documentation for a Digital Tutoring Platform as a service</p>

## Project Description
 
The pandemic demonstrated the potential of using digital services for small businesses. It showed that with the right customization, digital services for local services can be beneficial to their clients. 
 
Take for example freelance teachers/tutors. Specifically focusing on music teaching. 
 
Most music teachers either have their own teaching business or supplement their primary income with teaching services. These businesses usually serve a local area and the services from different teachers tend to be from a broad range of subjects. Some teachers offer music education in more than one instrument, while others are specialists in a specific form of music or musical instrument. Their fees also vary depending on demand, student skill level, and fixed costs. 
 
Some teachers prescribe a syllabus to work from for a structured approach to learning, usually an affiliated board. Students learn music theory, music history along-side their lessons on their instrument of choice. The aforementioned schools also hold routine exams to target completion of curriculum. Performance exams are held with external examiners certified by one of the schools. However, these aren't mandatory. A significant number of students are learning for fun and opt of these set patterns. 
 
The generic product aims to help freelance teachers and students by providing them with a digital interface. Teachers would be able to create a public board advertising their services and have a separate student only space that would cater to their student body. The students should be able to see messages, lesson summaries, recorded classes (if any), and progress reports. 
 
The product should be customizable depending on the services type. Depending on the affiliation, curriculum-based lessons plans should be pre-populated. More broadly, the product should have the ability to group teachers together to create institutions.
 
## Features:

1.	Public site for advertising services.
2.	Student portal to view lessons, access learning material, scheduling, and history.
3.	Social space to interact with other students - This would have custom features to upload work/performances/ session.
4.	Ability for teachers to upload content tailored to each student, moderate content, grade performances.
5.	Ability for teachers to broadcast internal messages, livestream classes.
6.	Ability to group teachers together to create larger institutions.




## Software Design Document | Use Case Diagram
![Use Case](./docs/assets/images/Use%20Case.png)



<details>
  <summary> Create New Public Page </summary>

| Description Item         | Description                                              |
|---------------------------|----------------------------------------------------------|
| Use Case ID               | 1                                                        |
| Use Case Description      | Also known as a public page - This is the landing page for all teachers offering their services |
| Actor                     | Teacher                                                  |
| Stakeholders and Needs    | Teacher - to have a digital public space that can be used to advertise services offered |
|                           | Visitor - to discover new teaching services               |
| Pre-conditions            | User with "Teacher" role has accessed the platform        |
| Trigger                   | Teacher clicks on create new public page                 |
| Post-conditions           | Teacher should have an SEO optimized public page offering teaching services in the local area |
| Basic flow                | 1. Teacher enters the name of the service                 |
|                           | 2. Teacher enters services being offered                  |
|                           | 3. Teacher enters the area of service offering           |
|                           | 4. Teacher enters prices of services being offered       |
|                           | 5. Teacher selects the color theme of the public page     |
|                           | 6. System generates a preview of the public page          |
|                           | 7. Teacher accepts the preview                            |
|                           | 8. Teacher selects the payment plan                        |
|                           | 9. Teacher pays the payment plan                           |
|                           | 10. Page is publicly available                             |
| Extensions                |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |
|                           |                                                          |


</details>


## Software Design Document | Sequence diagram

### Invitation flow
This flow is the starting point for most teachers. Admins would create invites for new teachers to sign up to the platform. They would also act as relationship managers to invitees that accept

<details>
  <summary> Invitation Flow </summary>

![Invite | Admin](./docs/assets/images/Sequence%20Diagram-Invite%20_%20Admin.png)

</details>

### Authentication flow
This is the most common authentication flow for all user roles on the platform. Using OAuth2 as a authentication platform, we can make do without some of the usual login processes for expediency
<details>
  <summary> Authentication Flow </summary>

![Authentication | Users](./docs/assets/images/Sequence%20Diagram-Authentication%20Flow%20_%20User.png)

</details>

### Teacher flow
Teachers will be able to create their own public pages, add in relevant content. They will also be able to create private rooms that is linked to each public room. This would be the student pages that would host the learning content

<details>
  <summary> Sign up </summary>

![Sign up | Teacher](./docs/assets/images/Sequence%20Diagram-Sign-up%20_%20Teacher.png)

</details>

<details>
  <summary> Create Public Room Flow </summary>

![Create Public Room | Teacher](./docs/assets/images/Sequence%20Diagram-Create%20Public%20Page%20_%20Teacher.png)


</details>

<details>
  <summary> Create Private Room Flow </summary>

![Create Private Room | Teacher](./docs/assets/images/Sequence%20Diagram-Create%20Private%20Page%20_%20Teacher.png)


</details>

<details>
  <summary> Manage Private Room Flow </summary>

![Manage Private Room | Teacher](./docs/assets/images/Sequence%20Diagram-Manage%20Class%20_%20Teacher.png)

</details>

### Student flow
Students will access private rooms with credentials provided by linked public room owners. There-fore each public room will have different login credentials.
<details>
  <summary> Student flow to view classes </summary>

![View Class | Student](./docs/assets/images/Sequence%20Diagram-View%20Class%20_%20Student.png)

</details>

### Visitor flow
<details>
  <summary> Enquiry flow for visitors </summary>
  
 
![Enquiry Flow | Visitor](./docs/assets/images/Sequence%20Diagram-Enquiry%20Flow%20_%20Visitor.png)

</details>


## Software Design Document | UML Class Diagram
![UML Class](./docs/assets/uml-classes.png)
