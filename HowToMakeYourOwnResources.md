# How to Create Your Own Interactive Classroom Resources with AI

[Back to list of activities](README.md)

Thanks to recent leaps in technology, you can now create interactive digital resources—like simulations, quizzes, and games—in the same amount of time it takes to make a standard worksheet.

This method uses "vibe-coding," where you describe the "vibe" or goal of what you want, and the AI handles the actual programming.

## Prerequisites

* **A Google Account:** You will need access to Google Gemini (available in all Google Workspace for Education accounts).
* **The Right Model:** Ensure you are using the **Gemini Advanced** (or "Pro") model for the best coding capabilities.
* **Hosting:** A place to upload your finished HTML files so students can access them (see the "How to Share" section at the end).

---

## Part 1: Design Your Activity

It helps to brainstorm with Gemini first, even if you already have an idea. This ensures the activity aligns perfectly with your lesson materials.

1. **Open Gemini:** Start a new chat.
2. **Upload Content:** Click the `+` or upload button to attach your course notes, slides, or a PDF of the topic you are teaching.
3. **Prompt for Ideas:** Ask Gemini to generate concepts based on your materials. You can use a prompt like this:

> "I want to create an interactive HTML page for **{A-Level Computer Science}** students demonstrating **{concept, e.g., the difference between fixed and variable length records}**.
> Please review the attached slides for the specific content and difficulty level. Suggest three ideas for an interactive activity. **DO NOT CODE ANYTHING YET.**"


1. **Refine the Idea:** Chat back and forth with Gemini until you settle on a specific activity you like.
* *Tip:* If you are teaching a complex topic, break it down. Ask for an activity covering just the first part. The more complex the task, the lower the chance you will get a working result.


5. **Create a "Spec Sheet":** Once you have an idea, ask Gemini to summarize it into a blueprint. This prevents the AI from forgetting details later.

> "Please create a specification document for the resource we just discussed. Include the learning objectives, target audience, key features, and a rough outline of the user interface."



---

## Part 2: Build the Resource

Now that you have a plan, it's time to let Gemini write the code.

1. **Start Coding:** Copy the "specification document" Gemini just wrote.
2. **Open Canvas:** Look for the **Canvas** or "Edit" mode in Gemini (this usually opens a dedicated window for code).
3. **The Build Prompt:** Paste your specification and add this instruction:

> "Please write the HTML code for this activity using the specification above. Create it as a single, self-contained HTML file with all CSS and JavaScript included."


1. **Test and Tweak:**
* Gemini will generate a preview. Click through it as if you were a student.
* If something isn't right, just tell Gemini plainly: *"The text is too small,"* *"The quiz gives the answer too quickly,"* or *"Make the buttons blue."*
* You can even take a screenshot of the error, paste it into the chat, and say, *"Fix this."*


5. **Download:** Once you are happy with the tool, click the download button (usually an arrow icon or "Download HTML") to save the file to your computer.

---

## Part 3: Host and Share (How to get it to students)

You now have an `.html` file on your computer, but your students need a web link to open it. Here are the easiest free ways to turn your file into a link without needing technical skills.

### Option 1: Tiiny.host (Easiest)

This is the simplest drag-and-drop solution.

1. Go to [Tiiny.host](https://tiiny.host/).
2. Drag your HTML file onto the homepage.
3. Type in a name for your link (e.g., `mr-smith-history-quiz`).
4. Click **Upload**. You will get a link you can immediately share on Google Classroom or email.

### Option 2: Static.app

Similar to Tiiny but offers a bit more control if you plan to make many resources.

1. Sign up for a free account at [Static.app](https://static.app/).
2. Drag and drop your file (or a folder of files) into the dashboard.
3. It will generate a public website link for you automatically.