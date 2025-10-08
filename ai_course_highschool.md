# Introduction to AI: A Hands-On Course for High School Students

## Course Overview
This course introduces high school students to AI through exciting, practical projects. Students will build real applications while learning core concepts of supervised and unsupervised learning. No advanced math required—just curiosity and creativity!

**Total Duration:** 8 modules (1 hour each)

---

## **Module 1: Welcome to AI - Your First Intelligent Program**
**Goal:** Get students excited and build something immediately

### Activities:
1. **Icebreaker (10 min):** Show AI fails and successes (funny TikTok filters, ChatGPT mistakes, amazing art generation)
2. **Hands-on Project (40 min):** Build a Movie Recommender
   - Use Teachable Machine (Google's no-code tool)
   - Train a model to recognize student facial expressions (happy/sad/surprised)
   - Connect it to recommend movies based on mood
   - **Tool:** Teachable Machine + simple HTML page
3. **Wrap-up (10 min):** Discuss "How did the computer learn?"

**Key Concept:** Machines learn from examples, just like humans!

---

## **Module 2: Supervised Learning - Teaching AI with Labels**
**Goal:** Understand classification through image recognition

### Activities:
1. **Hook (10 min):** Show how Snapchat filters work, medical diagnosis AI
2. **Hands-on Project (40 min):** Build a Recyclable vs. Trash Classifier
   - Students collect 20 images each of recyclables and trash (from their phones)
   - Upload to Teachable Machine
   - Train the model
   - Test with new items around the classroom
   - Export and run in browser
3. **Discussion (10 min):** 
   - What makes a good training example?
   - Why did it fail on [specific item]?
   - Real-world applications: Self-checkout, medical scans

**Key Concept:** Supervised learning = teaching with labeled examples

---

## **Module 3: Playing with Data - Your First Python AI**
**Goal:** Transition to code-based ML with simple, relatable data

### Activities:
1. **Demo (10 min):** Show how Netflix/Spotify predictions work
2. **Hands-on Project (40 min):** Predict Student Study Hours
   - Use Google Colab (no installation needed)
   - Dataset: Student hours studied vs. test scores (provided)
   - Use `scikit-learn` to build a simple linear regression
   - Students input THEIR study hours and get a prediction
   - Visualize with a graph
   
   ```python
   # Simple enough for beginners!
   from sklearn.linear_model import LinearRegression
   import matplotlib.pyplot as plt
   
   # Train model
   model.fit(hours_studied, test_scores)
   
   # Predict YOUR score
   my_hours = 5
   prediction = model.predict([[my_hours]])
   ```

3. **Challenge (10 min):** What other factors affect grades? (Sleep, phone time, etc.)

**Key Concept:** Regression = predicting numbers; more data = better predictions

---

## **Module 4: AI Can Decide - Classification Projects**
**Goal:** Build practical classification models

### Activities:
1. **Hook (10 min):** Show spam detection, fake news detection
2. **Hands-on Project (40 min):** Build a Text Message Spam Detector
   - Use Google Colab with pre-made dataset
   - Train model using `scikit-learn` (Naive Bayes)
   - Students test with real texts from their phones (privacy-conscious)
   - See the model's confidence scores
   
   **Extension:** Students create their own "fake" spam messages to fool the AI

3. **Discussion (10 min):** 
   - Can AI be biased? (Show examples)
   - Ethics: Should AI decide who gets loans? College admissions?

**Key Concept:** Classification = putting things into categories

---

## **Module 5: Unsupervised Learning - Finding Hidden Patterns**
**Goal:** Discover patterns without labels

### Activities:
1. **Hook (10 min):** How does Spotify create "Discover Weekly"? How do stores arrange products?
2. **Interactive Demo (15 min):** Clustering Candy
   - Physical activity: Give students mixed candies
   - Ask them to group without instructions
   - Discuss: Everyone grouped differently! (color, size, type)
   
3. **Hands-on Project (30 min):** Customer Segmentation Game
   - Dataset: Fictional students with (screen time, sports hours, music genre listens)
   - Use K-Means clustering to find "student types"
   - Visualize clusters
   - Students name each cluster ("The Gamers," "The Athletes," etc.)
   
4. **Wrap-up (5 min):** When is unsupervised learning useful?

**Key Concept:** Unsupervised learning = finding patterns without being told what to look for

---

## **Module 6: Making Recommendations - Build Your Own Netflix**
**Goal:** Combine concepts for a complex real-world application

### Activities:
1. **Hook (10 min):** Economics of recommendation systems (YouTube, TikTok, Amazon)
2. **Hands-on Project (45 min):** Build a Song Recommender
   - Use small dataset of song features (tempo, energy, danceability)
   - Implement content-based filtering (songs similar to ones you like)
   - Then simple collaborative filtering (songs liked by similar users)
   - Students rate 10 songs, get personalized recommendations
   
   **Tool:** Pre-built Colab notebook with simplified code

3. **Discussion (5 min):** Filter bubbles and echo chambers

**Key Concept:** Recommendation systems combine multiple AI techniques

---

## **Module 7: AI for Good - Social Impact Project**
**Goal:** Apply skills to meaningful problems

### Activities:
1. **Inspiration (15 min):** Show AI projects helping with:
   - Disaster response (damage detection from satellite images)
   - Accessibility (sign language translation)
   - Environment (species identification, pollution monitoring)

2. **Group Project Planning (45 min):**
   - Teams of 3-4 choose a problem:
     * **Plant disease detector** for local farmers
     * **Posture checker** for students studying
     * **Emotion detector** for mental health check-ins
     * **Noise level monitor** for classroom
   
   - Teams plan: What data? What model type? How to collect data?
   - Start building using Teachable Machine or Colab

**Key Concept:** AI as a tool for positive change

---

## **Module 8: Final Showcase + AI Futures**
**Goal:** Present projects and discuss AI's future

### Activities:
1. **Project Presentations (30 min):**
   - Each team demos their "AI for Good" project
   - Show successes AND failures (learning moments!)
   - Peer feedback

2. **AI Ethics Discussion (20 min):**
   - Deepfakes and misinformation
   - AI bias in hiring/policing
   - Will AI take jobs? Create jobs?
   - Student debates on regulation

3. **What's Next? (10 min):**
   - Resources for continued learning (Kaggle, fast.ai, YouTube channels)
   - AI career paths (research, engineering, ethics, policy)
   - Challenge: Build something over the summer!

**Key Concept:** With great AI power comes great responsibility

---

## **Required Tools & Resources**

### Software (All Free):
- **Google Teachable Machine** (no-code training)
- **Google Colab** (cloud Python environment)
- **Kaggle** (datasets and tutorials)
- Libraries: scikit-learn, pandas, matplotlib

### Datasets Provided:
- Student grades dataset
- SMS spam collection
- Song features dataset
- Sample images for classification

### Hardware:
- Computers with webcam
- Students' phones (for collecting images)
- Internet connection

---

## **Teaching Tips**

1. **Start Every Module with "Why Should I Care?"** - Show cool applications first
2. **Embrace Failure** - When models fail, that's the best teaching moment
3. **Make It Personal** - Use data about students themselves when possible
4. **Keep Code Simple** - Focus on understanding, not syntax
5. **Ethics Throughout** - Discuss bias, privacy, and impact regularly
6. **Encourage Creativity** - Let students modify projects with their own ideas

---

## **Assessment Ideas**

- **Participation:** Active engagement in hands-on activities
- **Mini-Quizzes:** Quick checks (supervised vs. unsupervised, when to use what)
- **Final Project:** "AI for Good" group project with presentation
- **Reflection Journal:** Weekly entries on "What surprised me?" and "Where can I apply this?"

---

## **Key Takeaways for Students**

By the end of this course, students will:
- ✅ Build 6+ AI projects they can show friends/family
- ✅ Understand when to use supervised vs. unsupervised learning
- ✅ Think critically about AI ethics and societal impact
- ✅ Have confidence to explore AI further on their own
- ✅ See AI as a creative tool, not magic

**Most importantly:** Students will be EXCITED about AI and see themselves as future AI creators, not just consumers!