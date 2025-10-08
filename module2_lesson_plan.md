# Module 2: Supervised Learning - Teaching AI with Labels
## Complete Lesson Plan

---

## **Overview**
- **Duration:** 60 minutes
- **Goal:** Understand classification through image recognition by building a practical recycling classifier
- **Key Concept:** Supervised learning = teaching with labeled examples
- **Tools Needed:** 
  - Computer with camera/webcam for each student
  - Smartphones (students bring their own)
  - Internet connection
  - Projector for demonstrations
  - Access to Teachable Machine (https://teachablemachine.withgoogle.com/)
  - Sample items: plastic bottle, paper, aluminum can, food wrapper, etc.

---

## **Lesson Timeline**

| Time | Activity | Duration |
|------|----------|----------|
| 0:00-0:10 | Hook: Real-World AI Applications | 10 min |
| 0:10-0:50 | Hands-on Project: Recyclable vs. Trash Classifier | 40 min |
| 0:50-1:00 | Discussion & Real-World Impact | 10 min |

---

## **Pre-Class Preparation**

### **Teacher Checklist (Day Before):**
- [ ] Send reminder for students to bring phones with cameras
- [ ] Collect sample items for demonstration (3-4 recyclables, 3-4 trash items)
- [ ] Test Teachable Machine on your device
- [ ] Prepare slideshow with examples of AI classification
- [ ] Have backup internet plan (hotspot)
- [ ] Print data collection worksheet (optional)

### **Materials Needed:**
- Sample recyclables: water bottle, soda can, cardboard box, paper
- Sample trash: chip bag, plastic wrap, styrofoam, candy wrapper
- Optional: Labels/sticky notes to mark items

---

## **Part 1: Hook - Real-World AI Applications (10 minutes)**

### **Teacher Script:**

> **[0:00-0:02] Opening Connection**
> 
> "Welcome back, AI creators! Last class, you built an emotion detector. Today, we're building something that could actually make money or help your school.
> 
> Quick question: Does anyone here actually enjoy sorting recycling from trash? Be honest!"
> 
> *[Students usually groan or laugh]*
> 
> "Yeah, nobody does. It's tedious, confusing—'Can I recycle this pizza box? What about this plastic bag?'—and when people get it wrong, it contaminates entire batches of recycling.
> 
> But what if AI could do it instantly? Just hold up an item, and boom—recycling or trash. That's what we're building today!"

---

> **[0:02-0:07] The Big Picture: Classification is Everywhere**
> 
> "Before we start, let me show you where this type of AI—called classification—is being used right now."
> 
> **SHOW EXAMPLES (slides/images):**
> 
> **1. Medical Diagnosis (Show X-ray with AI overlay)**
> "AI classifies X-rays as 'normal,' 'pneumonia,' or 'cancer.' In 2024, AI could detect lung cancer 2 years earlier than human radiologists in studies. Classification is literally saving lives."
> 
> **2. Self-Checkout Cameras (Show grocery store image)**
> "Ever use those 'scan your own items' machines? Cameras classify 'banana' vs 'avocado' vs 'apple' to prevent theft. Some stores report 20% of people try to scan expensive items as cheap ones!"
> 
> **3. Wildlife Conservation (Show camera trap image)**
> "Camera traps in rainforests classify animals: 'jaguar,' 'deer,' 'human poacher.' This helps protect endangered species without needing humans to watch thousands of hours of video."
> 
> **4. Content Moderation (Show social media icons)**
> "Platforms like Instagram use AI to classify images as 'safe,' 'violence,' 'inappropriate content.' It processes billions of images per day."
> 
> **5. Quality Control (Show factory image)**
> "Factories classify products as 'perfect' or 'defective.' AI can spot tiny cracks or defects humans might miss, at 1000x the speed."

---

> **[0:07-0:10] Today's Mission**
> 
> "All of these use supervised learning—the same technique from last class. The AI is shown thousands of labeled examples:
> - 'This is a recyclable'
> - 'This is trash'
> 
> After enough examples, it can classify things it's never seen before.
> 
> **Today's goal:** Build a working classifier that could be installed at your school's lunch room. By the end of class, you'll have an AI that can identify whether something belongs in recycling or trash.
> 
> But here's the catch—AI is only as smart as the data you give it. If you take sloppy photos or don't include enough variety, your AI will fail. You're scientists now, so we need GOOD data.
> 
> Phones out, everyone! Let's collect some data!"

---

## **Part 2: Hands-on Project - Build a Recycling Classifier (40 minutes)**

### **[0:10-0:15] Phase 1: Data Collection Strategy (5 min)**

### **Teacher Script:**

> "Before we start randomly taking pictures, let's think like data scientists. What makes GOOD training data?
> 
> *[Write on board while discussing]:*
> 
> **Good Training Data:**
> 1. **Variety** - Different angles, distances, lighting
> 2. **Representative** - Examples you'll actually encounter
> 3. **Clear labels** - No ambiguous items
> 4. **Balanced** - Equal amounts of each category
> 5. **Quality** - In focus, not blurry
> 
> Here's our plan:
> 
> **Recyclable Category - Collect 15-20 photos each of:**
> - Plastic bottles (water bottles, soda bottles)
> - Aluminum cans
> - Cardboard/paper
> - Glass bottles (if available)
> 
> **Trash Category - Collect 15-20 photos each of:**
> - Chip bags / snack wrappers
> - Plastic bags
> - Styrofoam
> - Mixed materials (like juice pouches)
> 
> **IMPORTANT RULES:**
> - Take photos from different angles (top, side, at an angle)
> - Different distances (close-up and far away)
> - Different backgrounds (desk, floor, hold it up)
> - Make sure items are IN FOCUS
> 
> You have 8 minutes to collect photos on your phones. GO!"

---

### **[0:15-0:23] Phase 2: Collect Photos (8 min)**

**Teacher Actions During This Time:**

1. **Circulate and coach:**
   - "That's too blurry—try again"
   - "Great! Now take one from the side"
   - "Is that background too messy? Try a plain surface"

2. **Take example photos yourself** to show later

3. **Check for common mistakes:**
   - All photos from same angle
   - Items too far away / too close
   - Fingers blocking the camera
   - Mixed categories (recyclable in trash pile)

4. **2-minute warning:** "You should have 10+ photos by now!"

**Troubleshooting:**

- **"I don't have any items!"** → Share items with neighbors, or use Google Images (but mark these differently)
- **"My phone camera isn't working!"** → Partner up or use webcam on computer
- **"Can I use photos from the internet?"** → Yes, but take SOME photos yourself for variety

---

### **[0:23-0:28] Phase 3: Set Up Teachable Machine (5 min)**

### **Teacher Script:**

> "Phones down! Let's get these photos into our AI.
> 
> **Everyone:**
> 1. Go to teachablemachine.withgoogle.com
> 2. Click 'Get Started' → 'Image Project' → 'Standard image model'
> 3. Rename 'Class 1' to 'Recyclable'
> 4. Rename 'Class 2' to 'Trash'
> 
> Now we need to upload your photos. You have two options:
> 
> **Option A: Transfer from phone**
> - Text photos to yourself
> - Email them to yourself
> - AirDrop (iPhone) or Nearby Share (Android)
> - Upload to Google Drive and download on computer
> 
> **Option B: Use webcam + hold items**
> - Click 'Webcam' button
> - Hold item in front of camera
> - Click 'Hold to Record'
> - Slowly rotate the item
> 
> I recommend Option B—it's faster! But if you took great photos on your phone, use Option A.
> 
> **Goal:** 50-100 images per category. You have 5 minutes!"

**Teacher Demo (while students work):**
- Show on projector: Uploading from phone OR using webcam
- Demonstrate holding item and rotating it
- Show the image counter increasing

---

### **[0:28-0:33] Phase 4: Train the Model (5 min)**

### **Teacher Script:**

> "Alright! If you have at least 40 images in each category, you're ready to train.
> 
> *[Check the room—help anyone who's behind]*
> 
> Now watch this magic happen. Everyone click the big blue **'Train Model'** button!
> 
> *[Students click, training begins]*
> 
> While it's training, let me explain what's happening inside the computer right now..."

---

> **[TEACHING MOMENT - While training runs]**
> 
> "Your computer is looking at ALL your images and finding patterns. It's asking questions like:
> 
> - What colors appear more in recyclables vs trash?
> - What shapes are common in each category?
> - What textures—smooth like plastic bottles or crinkly like chip bags?
> - Are there text or logos that indicate recyclability?
> 
> The AI isn't 'understanding' what recycling IS. It's finding mathematical patterns in pixels. It might notice:
> - Recyclables often have rigid edges and solid colors
> - Trash often has wrinkled surfaces and mixed colors
> 
> **But here's the key:** It ONLY learns what's in your training data. If you only took photos of Coca-Cola bottles, it might think all bottles are recyclable. If you only photographed Pepsi cans, it might not recognize a Red Bull can!
> 
> This is why big companies spend millions on training data. They need EVERY possible variation.
> 
> *[Training finishes—usually 30-60 seconds]*
> 
> Done! Let's test it!"

---

### **[0:33-0:43] Phase 5: Testing & Debugging (10 min)**

### **Teacher Script:**

> "Now the moment of truth. Look at the 'Preview' window on the right.
> 
> **Let's do a test together:**
> 1. Hold up a recyclable item you trained it on
> 2. What does it predict?
> 3. What's the confidence percentage?
> 
> *[Walk around and observe students testing]*
> 
> Now try to BREAK it! Here's your mission:
> 
> **Testing Challenge (5 minutes):**
> 1. Test an item you trained on ✓
> 2. Test an item you DIDN'T train on—does it work?
> 3. Test a tricky item (like a pizza box with grease, or a plastic bag)
> 4. Test with different backgrounds
> 5. Find ONE thing your AI gets completely wrong
> 
> As you test, write down:
> - What worked perfectly?
> - What failed miserably?
> - Why do you think it failed?
> 
> GO!"

---

**Teacher Actions During Testing:**

1. **Observe failures and highlight them:**
   - "Interesting! Sarah's AI thinks a paper plate is trash. Why might that be?"
   - "Jake's AI is 98% confident on this can. What made it so sure?"

2. **Collect examples for discussion:**
   - Note common failures to discuss
   - Identify edge cases students discover

3. **Prompt deeper thinking:**
   - "What would happen if you tested this under cafeteria lighting vs classroom lighting?"
   - "Would this work on crumpled items vs flat items?"

---

> **[0:38-0:43] Group Discussion of Results**
> 
> "Okay, testing time is up! Let's share what we discovered.
> 
> **Questions for class:**
> 
> 1. "Raise your hand if your AI got something WRONG."
>    *[Most hands go up]*
>    "Perfect! AI is never 100% accurate. What did yours get wrong?"
>    
>    *[Take 2-3 examples]:*
>    - Student 1: "It thought a notebook was recyclable"
>    - Student 2: "It couldn't tell if a plastic bag was trash"
>    - Student 3: "It said a soda can was trash!"
> 
> 2. "Why did it fail? Let's diagnose..."
>    *[Work through one example]:*
>    - "Did you have paper in your training data?"
>    - "Was your can crushed? Did you train it on crushed cans?"
>    - "Plastic bags are tricky—they're technically recyclable in some places but not others. The AI is confused because the LABEL is unclear!"
> 
> 3. "What would you need to make this work perfectly?"
>    *[Expected answers]:*
>    - More training data
>    - More variety in training data
>    - Test it in the actual environment (cafeteria)
>    - Maybe add a third category for "compost" or "uncertain"
> 
> This is EXACTLY what professional AI engineers do. They:
> 1. Build a model
> 2. Test it
> 3. Find failures
> 4. Collect more data to fix those failures
> 5. Repeat forever!
> 
> AI development is never 'done'—it's always improving."

---

### **[0:43-0:50] Phase 6: Deploy Your AI (7 min)**

### **Teacher Script:**

> "Your AI works! Now let's make it into a real application you could actually use.
> 
> Click 'Export Model' at the top, then 'Upload my model.'
> 
> *[Wait for uploads—this takes 1-2 minutes]*
> 
> Once it's uploaded, you'll get a link. Copy that link!
> 
> Now I'm going to share a simple website I built. You'll paste your model link into it, and boom—you have a working recycling scanner!
> 
> *[Share the HTML file - see artifact below]*
> 
> **Instructions:**
> 1. Download the file 'recycling-classifier.html'
> 2. Right-click → 'Open with' → Choose a text editor (Notepad, TextEdit, VS Code)
> 3. Find line 168: `const modelURL = "YOUR_MODEL_URL_HERE"`
> 4. Replace `YOUR_MODEL_URL_HERE` with your link (keep the `/model.json` at the end)
> 5. Save the file
> 6. Double-click the file—it opens in your browser
> 7. Test it with real items!
> 
> *[Students work on this while teacher circulates and helps]*
> 
> Once you have it working, try scanning different items around the classroom. You now have a portable AI-powered recycling assistant!"

---

## **Part 3: Wrap-up Discussion & Real-World Impact (10 minutes)**

### **[0:50-0:55] Discussion: When Does AI Fail?**

### **Teacher Script:**

> "Let's talk about what you just experienced. This wasn't just a fun project—you discovered some fundamental truths about AI.
> 
> **Question 1: What's the MOST important factor for good AI?**
> *[Expected answers: training data]*
> 
> Exactly! There's a saying in AI: 'Garbage in, garbage out.' The best algorithm in the world can't fix bad data.
> 
> **Question 2: Did anyone's AI get confused on something that was OBVIOUS to you?**
> *[Take examples—like mistaking paper towel for paper]*
> 
> This shows a key limitation: AI doesn't 'understand' context. You know a greasy paper towel shouldn't be recycled, even though it's paper. The AI just sees 'paper-like texture' and guesses.
> 
> **Question 3: Could this AI be biased or unfair?**
> 
> Think about it: If you only trained on items from American stores, would it work in Japan? If you only photographed items in bright daylight, would it work in dim cafeteria lighting?
> 
> This is how bias creeps into AI:
> - Medical AI trained mostly on light-skinned patients → fails on dark-skinned patients
> - Voice assistants trained on American accents → fails on other accents
> - Job screening AI trained on male resumes → discriminates against women
> 
> It's not because the AI is 'racist' or 'sexist'—it's because the TRAINING DATA was limited!"

---

### **[0:55-0:58] Real-World Impact**

### **Teacher Script:**

> "Now the exciting part: This technology is being deployed RIGHT NOW.
> 
> **1. AMP Robotics** (Show logo/image)
> - Uses AI vision + robot arms to sort recycling
> - Can sort 160 items per minute (twice as fast as humans)
> - Reduces contamination by 50%
> - Your project was a simplified version of this!
> 
> **2. Oscar the Smart Trash Can**
> - Installed in some offices/airports
> - You hold up item, camera classifies it, correct door opens
> - Improved recycling accuracy from 20% to 85%
> 
> **3. Google Lens**
> - Point camera at any object, it identifies it
> - Same classification technique you just used
> - Trained on billions of images
> 
> **The Business Case:**
> - Contaminated recycling costs cities millions (entire trucks get dumped as trash)
> - If your school installed this, it could:
>   * Reduce waste disposal costs
>   * Increase recycling revenue
>   * Teach students about sustainability
> 
> Some schools are already doing this! In 2024, a high school in California built a similar system and reduced their trash by 30%."

---

### **[0:58-1:00] Homework & Preview**

### **Teacher Script:**

> "Amazing work today! You're now experts in classification AI.
> 
> **Optional Homework:**
> 1. Show your family your recycling classifier
> 2. Test it at home—does it work on YOUR family's trash?
> 3. Think about: What else could we classify?
>    - Ripe fruit vs unripe
>    - Weeds vs garden plants
>    - Counterfeit products vs real ones
> 
> **Next Class Preview:**
> Next time, we're leveling up to Python! You'll write actual code to build an AI that can predict YOUR test scores based on study hours. We're going from no-code to real code.
> 
> Don't worry—I'll guide you through every step. If you want to get a head start, create a free Google Colab account at colab.research.google.com.
> 
> Great job today, AI engineers! You built something that could genuinely help your school!"

---

## **Assessment Rubric**

### **Participation (40 points)**
- [ ] Collected diverse training photos (10 pts)
- [ ] Successfully trained model (10 pts)
- [ ] Tested model and identified failures (10 pts)
- [ ] Participated in class discussions (10 pts)

### **Understanding (40 points)**
- [ ] Can explain what supervised learning means (10 pts)
- [ ] Understands importance of training data quality (10 pts)
- [ ] Can identify why AI might fail (10 pts)
- [ ] Recognizes potential for AI bias (10 pts)

### **Technical Skills (20 points)**
- [ ] Successfully used Teachable Machine (10 pts)
- [ ] Deployed model to HTML page (10 pts)

### **Bonus Points (up to 10)**
- Found creative edge cases (5 pts)
- Helped classmates troubleshoot (5 pts)
- Asked insightful questions (5 pts)

**Total: 100 points possible**

---

## **Common Issues & Solutions**

### **Technical Problems**

| Problem | Solution |
|---------|----------|
| "Photos won't upload from phone" | Use webcam option instead; hold items in front of camera |
| "Model keeps saying 'Trash' for everything" | Likely unbalanced data—check if one category has way more images |
| "Training is stuck at 50%" | Refresh page and retrain; reduce number of images if needed |
| "Webcam shows items but predictions are random" | Not enough training data; need at least 40 images per category |
| "Can't export model" | Try 'Download' instead of 'Upload'; can share model file via cloud |

### **Pedagogical Challenges**

**Problem: "Students rushing through data collection"**
- **Solution:** Stop class after 5 minutes, show examples of good vs bad photos on projector
- Do a "data quality check" where you review a few students' photos

**Problem: "AI working TOO well, students not experiencing failure"**
- **Solution:** Intentionally introduce a challenging item (like a paper plate)
- Ask: "What would happen if we tested this in the dark?"

**Problem: "Students frustrated by low accuracy"**
- **Reframe:** "Perfect! You just learned what professional AI engineers deal with. How would you fix it?"
- Celebrate failure as learning

---

## **Extension Activities**

### **For Students Who Finish Early:**

1. **Add More Categories:**
   - Compost
   - E-waste
   - Hazardous materials

2. **Test Edge Cases:**
   - Wet vs dry items
   - Clean vs dirty items
   - Whole vs crushed items

3. **Improve the Model:**
   - Collect 50 more images
   - Retrain and compare accuracy

4. **Document Failures:**
   - Create a "failure log" with photos
   - Hypothesize why each failed
   - Suggest fixes

5. **Real-World Research:**
   - Find 3 companies using AI for recycling
   - What accuracy do they claim?
   - How much do their systems cost?

---

## **Materials Checklist**

### **Before Class:**
- [ ] Sample recyclables (5-10 items)
- [ ] Sample trash (5-10 items)
- [ ] Slideshow with real-world examples
- [ ] HTML template file ready to share
- [ ] Test Teachable Machine yourself
- [ ] Backup internet (hotspot)

### **During Class:**
- [ ] Projector working
- [ ] All computers have webcam access
- [ ] Students have phones (or backup webcams)
- [ ] Items easily accessible for testing

### **To Share Digitally:**
- [ ] Link to Teachable Machine
- [ ] HTML template file
- [ ] Optional: Example images for students without items

---

## **Key Takeaways for Students**

By the end of this module, students should be able to:

✅ **Define** supervised learning (learning from labeled examples)
✅ **Explain** why training data quality matters ("garbage in, garbage out")
✅ **Build** an image classification model from scratch
✅ **Test** and debug an AI model
✅ **Identify** limitations and failure modes of AI
✅ **Recognize** how AI bias originates from training data
✅ **Connect** classroom project to real-world applications
✅ **Think critically** about when AI is appropriate vs inappropriate

---

## **Teacher Reflection Notes**

*[Fill out after teaching]*

**What worked well:**
- 
- 

**What to adjust next time:**
- 
- 

**Student insights that surprised me:**
- 
- 

**Time management notes:**
- Section that took longer than expected:
- Section that went faster:

**Technical issues encountered:**
- 
- 

**Best student questions:**
- 
-