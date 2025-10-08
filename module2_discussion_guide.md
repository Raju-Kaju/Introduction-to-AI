# Module 2: Discussion Prompts & Troubleshooting Guide

## Deep Discussion Questions

### Use these throughout the lesson to stimulate critical thinking

---

## **Section 1: Understanding Classification**

### Question Set 1: The Nature of Learning

**Q: "How does the AI actually 'see' the difference between recyclable and trash?"**

**Expected Student Answers:**
- "It looks at the shape"
- "It recognizes colors"
- "It reads labels"

**Teacher Follow-Up:**
"Close! The AI doesn't 'see' like we do. It converts the image into millions of numbers (pixel values), then finds mathematical patterns. It might notice 'recyclables have more blue pixels' or 'trash has more irregular edges.' But it doesn't 'understand' what recycling IS—it just finds correlations in the numbers."

**Key Concept to Emphasize:** AI is pattern matching, not understanding.

---

**Q: "Could this AI work in the dark? Why or why not?"**

**Expected Student Answers:**
- "No, you can't see anything"
- "Maybe if it has night vision"

**Teacher Follow-Up:**
"Great thinking! This is actually a HUGE issue in AI deployment. If you trained your model in bright classroom lights, it might fail in dim cafeteria lighting. This is called 'distribution shift'—the real-world data looks different from training data.

Real solution? Either:
1. Train with data in various lighting conditions
2. Add infrared cameras
3. Control lighting in deployment environment

This is why self-driving cars struggle in rain/snow—most training data is sunny California!"

**Key Concept to Emphasize:** Training environment must match deployment environment.

---

### Question Set 2: Data Quality

**Q: "What would happen if you only took photos of Coke bottles for recyclables?"**

**Expected Student Answers:**
- "It would only recognize Coke bottles"
- "It might think red = recyclable"

**Teacher Follow-Up:**
"Exactly! This is called 'overfitting'—the AI learns too specific patterns. It might think:
- Red + white logo = recyclable
- Curved shape = recyclable

Then it would classify red trash items as recyclable! This is why diversity in training data is crucial.

Real example: Amazon's hiring AI trained on past successful candidates (mostly male) started discriminating against female candidates. The AI learned 'male patterns' instead of 'good employee patterns.'"

**Key Concept to Emphasize:** Diverse data prevents overfitting and bias.

---

**Q: "Is it better to have 1000 photos of one item, or 10 photos each of 100 different items?"**

**Expected Student Answers:**
- Usually split, some say 1000 of one

**Teacher Follow-Up:**
"Great question! Generally, 100 different items is MUCH better. Here's why:

**1000 of one item:**
- AI becomes expert on THAT item
- Fails on anything different
- Called 'overfitting'

**10 each of 100 items:**
- AI learns general patterns of the CATEGORY
- Works on items it's never seen
- Called 'generalization'

However, you need ENOUGH examples of each—10 might not be enough. Professional models use thousands of examples of hundreds of categories.

Rule of thumb: Breadth > Depth (to a point)"

**Key Concept to Emphasize:** Generalization requires diversity, not just quantity.

---

## **Section 2: Ethics & Bias**

### Question Set 3: Fairness in AI

**Q: "Could your recycling AI be unfair or biased? How?"**

**Prompt if needed:** "What if you only trained on American products?"

**Expected Student Answers:**
- "It wouldn't work on products from other countries"
- "Different recycling symbols in different countries"

**Teacher Follow-Up:**
"Brilliant! This is REAL bias in AI. Let's think deeper:

**Geographic bias:**
- US uses numbered triangle symbols
- Europe uses different symbols
- Japan has yet another system
- Your AI trained on US products fails globally

**Socioeconomic bias:**
- Trained on name-brand items?
- Might fail on generic/off-brand packaging
- Could unfairly flag certain communities' items as 'uncertain'

**Temporal bias:**
- Trained on 2024 packaging?
- Won't work on 2030 packaging when designs change
- Needs continuous retraining

This isn't theoretical—facial recognition trained mostly on light-skinned faces had up to 34% higher error rates on dark-skinned faces (MIT study, 2018)."

**Key Concept to Emphasize:** Bias comes from training data, not bad intentions.

---

**Q: "Should schools use AI to sort recycling automatically?"**

**Present Scenario:**
"Imagine your school installs an AI sorting system. It costs $50,000 but could:
- Reduce contamination by 70%
- Save $10,000/year in waste costs
- Teach students about technology

But:
- It fails 15% of the time
- Contaminated recycling still happens
- Might replace student recycling volunteers

**Debate:** Is this worth it?"

**Facilitate Both Sides:**

**Pro AI:**
- Better accuracy than humans over time
- Cost savings can fund other programs
- Educational value
- Consistency (doesn't get tired/lazy)

**Anti AI:**
- 15% failure rate is significant
- Humans can think contextually (greasy pizza box)
- Loss of student engagement/jobs
- What if it breaks? Need human backup anyway

**Teacher Conclusion:**
"There's no clear answer! This is real AI ethics. Companies and cities make these decisions daily. The key is:
1. Understand the trade-offs
2. Plan for failures
3. Keep humans in the loop for hard cases
4. Continuously monitor and improve"

**Key Concept to Emphasize:** AI is a tool; humans decide if/how to use it.

---

## **Section 3: Real-World Connections**

### Question Set 4: Scaling Up

**Q: "What would it take to make your AI work in the school cafeteria?"**

**Brainstorm with Students (write on board):**

**Technical Requirements:**
- More training data (thousands of images)
- Images from cafeteria (different lighting)
- All types of items students bring
- Different angles (overhead camera? side camera?)
- Fast processing (real-time classification)
- High-resolution camera

**Practical Requirements:**
- Where to mount camera?
- How do students use it?
- What happens when it's wrong?
- Who maintains it?
- How to handle edge cases?

**Cost Analysis:**
- Camera: $200-500
- Computer: $500-1000
- Installation: $500
- Training time: 20 hours
- Maintenance: $1000/year

**Total:** ~$3000 initial + ongoing

**Is it worth it?** Depends on:
- How much contamination costs now
- School budget
- Student buy-in

**Key Concept to Emphasize:** Moving from prototype to production is complex.

---

**Q: "Where else could classification AI be used at school?"**

**Student Brainstorm (encourage creativity!):**

Possible answers:
- **Library:** Classify books by genre from cover photos
- **Lost & Found:** Match found items to descriptions
- **Science Lab:** Identify plants, rocks, chemicals
- **Art Class:** Classify art styles
- **PE:** Posture correction for exercises
- **Safety:** Detect if someone is wearing required equipment
- **Attendance:** Facial recognition (discuss ethics!)
- **Food Service:** Identify allergens in dishes

**For Each Idea, Ask:**
1. What would you need to train it?
2. What could go wrong?
3. Is this a good use of AI, or should humans do it?

**Key Concept to Emphasize:** AI is versatile but not always the best solution.

---

## **Section 4: Failure Analysis**

### Question Set 5: Debugging Thinking

**Present Common Failure Scenarios:**

**Scenario 1: "My AI says everything is recyclable"**

**Diagnostic Questions:**
- How many images in each category?
- Are the images balanced?
- Did you accidentally put trash images in recyclable category?

**Most Common Cause:** Unbalanced data (e.g., 200 recyclable images, 20 trash images)

**Fix:** Balance the data, retrain

---

**