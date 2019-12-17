---
title: "Author and student views"


---

The experience when authoring differs from that of a student. Students are not able to view the authoring tools. When they start a unit or project, if there is content present, it will automatically be shown. The author can also specify whether the student is able to close the content or not.

If you are an author, you will often want to view the content as a student will see it.

# Editing
Only an author is able to edit the content. Students and users with read-only rights will not be able to. [Click here](/content/authoring/page-edit) for details on page editing.

# Preview
You can press the preview button in the top right area of the edit pane. This will switch to preview mode. You can then switch back to editor mode by pressing the **Editor** button.

You can also start the preview mode from the **Tools->Guide->Play**.

Finally, there is also a button at the top of the file tree that launches the content.


![StartGuides](/img/guides/startguides.png)

<a name="customisetopmenu"></a>
# Customising IDE menu
To simplify the educational process for students, the top menu can be customised to remove options from students that they cannot override.


Through a `.codio-menu` file, a teacher can specify what menu items should be hidden.
Example:

```json
{
    "Logo": false, // hides the Codio logo
	"Codio": false, // hides the Codio menu dropdown
    "Project": {
         "Permissions": false // hides the Permissions option in the Project menu dropdown
    },
    "Help": false, // hides the Help menu dropdown
    "Run": false, // hides the Run menu dropdown
    "Preview": false, // hides the Preview menu dropdown
    "Debugger": false, // hides the Debugger menu dropdown
    "Status": false // hides the Status icon, user Avatar, user name and exit button
}
```

**Please note that if setting Status=false, students will need to use the 'Back to Dashboard' button shown on the last page of the guides to return to their dashboard area**

Setting up .codio-menu file:

![EditorMode](/img/guides/codiomenu.png)

Menu items that the student will see:

![PreviewMode](/img/guides/codiomenupreview.png)

The student will not see the .codio-menu file to be able to edit/change it.

# Player Options
![authtoken](/img/guides/playmode.png)

When the content is rendered to a student, various options can be controlled

- The **Collapse table of contents**  button allows the user to collapse the content pane to provide larger working area if required.
- **Navigation Buttons** allows the user to navigate forward/backward in the guide.
- **Settings** allows the user to view the unit as a teacher (e.g. show solution information hidden to students) change the Theme (light/dyslexic), Mark as Complete, change the font size, reset both the theme and fonts and to restore the current files (see below). See [Dyslexia Support](/dashboard/student/dyslexia/) section
- **[Show/Hide Section List Hamburger Icon](/content/authoring/guides/collapse/)** allows the user to show/hide the section list.

## Restore current files
The Restore Current Files feature is a great way to reset/restore any files on that page to its initial state after hacking sample code around. Files can be restored from the menu as shown below.

![authtoken](/img/guides/reset.png)

