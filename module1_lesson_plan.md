# Module 1: Welcome to AI - Your First Intelligent Program
## Complete Lesson Plan

---

## **Overview**
- **Duration:** 60 minutes
- **Goal:** Get students excited about AI and build their first intelligent program
- **Key Concept:** Machines learn from examples, just like humans!
- **Tools Needed:** 
  - Computer with webcam for each student (or pairs)
  - Internet connection
  - Projector for demonstrations
  - Access to Teachable Machine (https://teachablemachine.withgoogle.com/)

---

## **Lesson Timeline**

| Time | Activity | Duration |
|------|----------|----------|
| 0:00-0:10 | Icebreaker: AI in Your Life | 10 min |
| 0:10-0:50 | Hands-on Project: Mood-Based Movie Recommender | 40 min |
| 0:50-1:00 | Wrap-up Discussion & Preview | 10 min |

---

## **Part 1: Icebreaker - AI in Your Life (10 minutes)**

### **Teacher Script:**

> **[0:00-0:02] Opening Hook**
> 
> "Good morning everyone! Quick question: How many of you used AI today before coming to class? Show of hands!"
> 
> *[Wait for responses, students usually say no or look confused]*
> 
> "Really? Let me ask differently: Did anyone check their phone this morning? Use face unlock? Get a suggested reply on a text? See a recommended video on YouTube or TikTok? Hear a song on Spotify you didn't search for?"
> 
> *[Students realize: "Oh! That's ALL AI!"]*
> 
> "Exactly! AI is everywhere, but most of it is invisible. Today, we're going to pull back the curtain and build our own AI—from scratch. And here's the best part: you don't need to be a math genius or a coding expert. You just need to teach a computer, kind of like training a pet."

> **[0:02-0:07] Show & Tell: AI Wins and Fails**
> 
> "Before we build, let's see what AI can do—both amazing and hilarious. I'm going to show you some examples."
> 
> **SHOW VIDEO/IMAGES:**
> 1. **AI Win:** Medical AI detecting cancer earlier than doctors
> 2. **AI Fail:** Google Photos tagging Black people as gorillas (2015)
> 3. **AI Fun:** Snapchat filters making you look like a potato
> 4. **AI Controversial:** AI-generated art winning art competitions
> 5. **AI Weird:** ChatGPT confidently giving wrong answers
> 
> "What do all these have in common? The AI learned from examples. Sometimes it learned the right things, sometimes it learned the wrong things, and sometimes it learned weird things. Today, YOU become the teacher."

> **[0:07-0:10] The Challenge**
> 
> "Here's what we're building today: an AI that can read your face and recommend movies based on your mood. Feeling sad? It'll suggest a comedy. Happy? Maybe an action movie. Surprised? A thriller!
> 
> By the end of this class, you'll have a working AI that you can take home and show your family. Ready? Let's go!"

---

## **Part 2: Hands-on Project - Mood-Based Movie Recommender (40 minutes)**

### **[0:10-0:15] Introduction to Teachable Machine (5 min)**

### **Teacher Script:**

> "We're using a tool called Teachable Machine by Google. It's like training wheels for AI—no coding required for now.
> 
> Think of it like this: When you were little, someone showed you pictures and said 'dog,' 'cat,' 'bird.' After seeing enough examples, you could recognize new animals you'd never seen before. That's exactly what we're doing with the computer.
> 
> **Everyone, open your browsers and go to: teachablemachine.withgoogle.com**
> 
> Click on 'Get Started,' then choose 'Image Project,' then 'Standard image model.'"

### **Step-by-Step Instructions (Displayed on Screen):**

```
STEP 1: Set Up Your Classes
- You should see "Class 1" and "Class 2"
- Click "Add a class" to make a third one
- Rename them:
  * Class 1 → "Happy"
  * Class 2 → "Sad"  
  * Class 3 → "Surprised"
```

---

### **[0:15-0:30] Training the Model (15 min)**

### **Teacher Script:**

> "Now comes the fun part—teaching the AI! You're going to give it examples of what you look like when you're happy, sad, and surprised.
> 
> **Important tips:**
> 1. Make CLEAR facial expressions—exaggerate them!
> 2. Move your head slightly while recording (left, right, closer, farther)
> 3. We want about 100-150 images per emotion
> 4. The AI learns better with variety
> 
> **Let's do 'Happy' together:**
> - Click the 'Webcam' button under 'Happy'
> - Make your biggest smile
> - Click 'Hold to Record' and keep smiling while moving slightly
> - Count to 5... DONE!
> 
> **Now you do the other two emotions on your own. I'll give you 5 minutes. Go!**"

### **Troubleshooting (Circulate & Help):**
- **"My webcam isn't working!"** → Check browser permissions (usually a popup)
- **"Do I need to make the same face every time?"** → No! Variety helps the AI learn better
- **"Can I wear glasses/hat?"** → Yes! That makes it more realistic

---

### **[0:30-0:35] Train the AI (5 min)**

### **Teacher Script:**

> "Alright, everyone should have images for all three emotions. Now watch this magic happen.
> 
> See that big blue button that says 'Train Model'? Click it!
> 
> *[Students click, progress bar appears]*
> 
> What's happening right now? The computer is looking at ALL your photos and finding patterns. It's figuring out:
> - 'Oh, when this person is happy, their mouth curves up and their eyes squint'
> - 'When they're sad, their mouth curves down'
> - 'When they're surprised, their eyes get wide and mouth opens'
> 
> It's doing this with millions of tiny calculations—finding the mathematical patterns in your face. But you don't need to understand the math, just like you don't need to understand how a car engine works to drive.
> 
> *[Training finishes—usually 20-30 seconds]*
> 
> Done! Now let's test it!"

---

### **[0:35-0:40] Testing (5 min)**

### **Teacher Script:**

> "Look at the 'Preview' panel on the right. Make a happy face... what does it say?
> 
> *[Students test, get excited when it works]*
> 
> Now try to TRICK it! Can you make a face it gets wrong?
> 
> *[Let students experiment]*
> 
> **Questions to ask while they test:**
> - Why do you think it got that wrong?
> - What could we do to make it better?
> - Would it work on your friend's face, or only yours?
> 
> *[Explain: It's trained on YOUR face, so it works best for you. To work for everyone, we'd need thousands of different faces in training—which is what Snapchat and Face ID actually do!]*"

---

### **[0:40-0:50] Add Movie Recommendations (10 min)**

### **Teacher Script:**

> "Okay, we have an AI that can read emotions. But we wanted it to recommend MOVIES, right? Let's connect the dots!
> 
> Click on 'Export Model' at the top, then choose 'Upload my model.' Give it a minute to process.
> 
> *[While it uploads]*
> 
> What it's doing is putting your AI 'brain' on the cloud so we can use it in a website. Once it's done, you'll get a link—copy that link!"

### **Now Use the HTML Code:**

> "I've created a simple website that connects to your AI. We're going to download it and plug in your model.
> 
> **[Share the HTML file with students - see artifact below]**
> 
> 1. Download the file 'movie-recommender.html'
> 2. Open it in a text editor (Notepad, TextEdit, or VS Code)
> 3. Find the line that says `YOUR_MODEL_URL_HERE`
> 4. Replace it with the link you copied
> 5. Save the file
> 6. Double-click the file—it opens in your browser!
> 
> Now try different expressions. It should show movie recommendations based on your mood!"

---

## **Part 3: Wrap-up Discussion (10 minutes)**

### **Teacher Script:**

> **[0:50-0:55] Debrief**
> 
> "Alright, let's talk about what just happened. You just built artificial intelligence! Let me ask you some questions:
> 
> **Question 1:** How did the computer learn to recognize your emotions?
> *[Expected answer: From the examples we gave it]*
> 
> Exactly! This is called **supervised learning**—you supervised the learning by giving it labeled examples. You said 'This is happy, this is sad, this is surprised.'
> 
> **Question 2:** Why doesn't it work perfectly every time?
> *[Let students discuss: not enough examples, expressions weren't clear, lighting changed, etc.]*
> 
> Right! AI is only as good as the data you give it. Garbage in, garbage out.
> 
> **Question 3:** Could this AI be biased or unfair?
> *[Prompt thinking: What if you only trained it on smiling happy faces? What if you only used photos of one race/gender?]*
> 
> This is HUGE in real AI. If you train an AI only on data from one type of person, it won't work well for others. This has happened with facial recognition failing on darker skin tones because it was trained mostly on white faces."

> **[0:55-0:58] Real-World Connections**
> 
> "Where is this used in real life?
> - **Snapchat/Instagram filters** - exact same tech
> - **Face ID on your phone** - recognizing YOUR face specifically
> - **Security cameras** - detecting suspicious behavior
> - **Car safety systems** - seeing if driver is drowsy
> - **Video game emotion** - NPCs reacting to player expressions
> 
> The difference? Those companies have MILLIONS of examples and way more computing power. But the core idea? Identical to what you just did."

> **[0:58-1:00] Preview Next Class**
> 
> "Next class, we're leveling up. We're going to build something that could actually help your school: a Recyclable vs. Trash classifier. Bring your phones—we'll need to take photos!
> 
> **Homework (Optional but Fun):**
> - Show your family what you built
> - Think about: What else could we teach a computer to recognize?
> - Can you think of problems at school or home that AI could solve?
> 
> See you next time! You're officially AI creators now!"

---

## **Assessment Checklist**

During class, observe and check off:
- [ ] Student successfully created three classes in Teachable Machine
- [ ] Student collected training data (images) for each emotion
- [ ] Student trained the model and tested it
- [ ] Student engaged in discussion about how the AI learns
- [ ] Student successfully exported and connected their model to the HTML page

**Participation Points:**
- Full credit for active participation and completing the project
- Bonus for: Creative expressions, helping peers, asking insightful questions

---

## **Common Issues & Solutions**

| Problem | Solution |
|---------|----------|
| "Webcam not working" | Check browser permissions; try different browser (Chrome works best) |
| "Training is taking forever" | Check internet connection; try reducing number of samples to 50 per class |
| "AI keeps getting it wrong" | Need more varied training data; make expressions more exaggerated |
| "Export button not working" | Model may still be training; wait for "Model trained!" message |
| "HTML file not opening model" | Check URL is pasted correctly with no spaces; ensure internet connection |

---

## **Extension Activities**

**For students who finish early:**

1. **Add more emotions:** Try "Angry," "Confused," "Excited"
2. **Test on others:** Does it work on your classmate's face? Why or why not?
3. **Break it:** Try to find what makes it fail (sunglasses, weird angle, low light)
4. **Different application:** Instead of movies, recommend songs or food

---

## **Teacher Preparation Checklist**

**Before Class:**
- [ ] Test Teachable Machine on your device
- [ ] Ensure all student computers have webcam access
- [ ] Download and test the HTML file
- [ ] Prepare examples of AI wins/fails to show
- [ ] Create backup plan if internet is unstable (can use Teachable Machine offline mode)
- [ ] Have movie list ready for recommendations

**Materials to Share:**
- [ ] Link to Teachable Machine
- [ ] HTML template file
- [ ] List of movies for each mood (or let students decide)

---

## **Learning Objectives - Did Students...**

✅ **Understand** that AI learns from examples (supervised learning)
✅ **Experience** the complete AI development cycle (collect data → train → test → deploy)
✅ **Recognize** that AI quality depends on training data quality
✅ **Connect** the project to real-world applications
✅ **Begin thinking** about AI ethics and bias
✅ **Feel excited** and empowered to build more AI projects

---

## **Notes for Future Improvements**

*[Teacher: Fill this out after teaching]*

**What worked well:**
- 
- 

**What to change next time:**
- 
- 

**Student questions I couldn't answer:**
- 
- 

**Time adjustments needed:**
- 
-