---
title: "LTI Class fork"


---
Enabling this setting allows existing Codio class content used in your LMS to be forked into a new Codio class and a new course in your LMS. This should be enabled for the classes connected with the "Master" course in your LMS. The parameter will be disabled by default for for all forked classes.

**Please note the screenshots below are for implementation in Canvas but other LMS systems should be similar. Refer to their documentation for more assistance**

First enable [LTI Constant URLs](/classes/lti/lti1_0/lticonstanturl) for your class.

- In your existing Codio class, enable the **Enable LTI class fork** button, and save your changes

![Enable Class fork field](/img/lti/enable_class_fork.png)

- In your LMS "Copy this Course" (or equivalent term for your LMS) and create your new course

![Copy LMS Course](/img/lti/copy_course.png)

- When completed go to **External Apps** and edit the existing app connecting Codio to your LMS
- Replace the existing custom field that was set from your original Codio class with an id of your own (e.g something like codio_class_target_id=my_class_id_10)

**N.B. If you LMS supports `lis_course_offering_sourcedid` you do not need to specify `codio_class_target_id` for the forked class, `lis_course_offering_sourcedid` will be used automatically to detect the course**

![Class fork id](/img/lti/fork_class_id.png)

- In your existing Codio class, copy the content of the LTI class fork enabled field into a new line in the 'Edit App' custom field
![Parent Class ID](/img/lti/parent_class.png)
- Submit

- In the new course created in your LMS, open one of the new assignments and this will then create the new class in Codio containing the content from your original Codio class.


