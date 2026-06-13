Step 1: User Flow
Daily Check-in

Student opens app and sees:

How are you feeling today?

😄 Great
🙂 Good
😐 Okay
😔 Stressed
😢 Exhausted

Then:

Write freely about your day...

Example:

I studied Physics for 8 hours.
I couldn't solve mock test questions.
Feeling anxious about NEET.
Parents are expecting a high score.
Step 2: AI Analysis

Prompt sends journal entry to Gemini.

AI extracts:

{
  "emotion":"anxiety",
  "stress_level":8,
  "confidence_level":3,
  "burnout_risk":"medium",
  "triggers":[
     "mock test performance",
     "parental pressure"
  ]
}
Step 3: Personalized Response

Instead of generic advice:

Bad:

Don't worry.
Stay positive.

Good:

You seem particularly worried about mock-test performance.

Students often interpret one difficult test as a reflection
of their final exam outcome.

For today:
✓ Stop studying after 10 PM
✓ Spend 15 mins reviewing mistakes
✓ Avoid taking another mock test tonight
✓ Try a 3-minute breathing exercise
Step 4: Pattern Detection

Store all journals.

After 7 days:

AI identifies:

Most common trigger:
Mock Tests

Highest stress day:
Sunday

Best mood day:
After Biology revision

Sleep issue detected:
Last 4 entries mention late-night study.

This is where judges usually get impressed.

Core AI Prompt

System Prompt:

You are MindMate AI, an empathetic mental wellness coach
for students preparing for competitive examinations.

Your role:

1. Analyze journal entries.
2. Detect emotions.
3. Detect stress triggers.
4. Detect burnout signs.
5. Identify confidence levels.
6. Provide personalized support.
7. Never diagnose mental illness.
8. Never claim to be a therapist.
9. Encourage professional help if severe distress is detected.

Return JSON only.

Schema:

{
 "emotion":"",
 "stress_level":"",
 "confidence_level":"",
 "burnout_risk":"",
 "triggers":[],
 "support_message":"",
 "coping_strategy":[]
}
Pattern Analysis Prompt

Every week:

Analyze these 7 journal entries.

Find:

1. Repeating emotional patterns
2. Common stress triggers
3. Burnout indicators
4. Motivation trends
5. Study-life imbalance
6. Positive habits

Return actionable insights.
Advanced Prompt (Hackathon Winning)

Instead of analyzing only today's journal:

Send:

Today's Entry:
{{journal}}

Previous 7 Day Summary:
{{memory}}

Exam:
NEET

Days Left:
45

Ask Gemini:

Generate personalized wellness guidance
based on today's emotions,
past emotional history,
and upcoming exam pressure.

Now AI feels "memory-aware."

Emergency Risk Detection

Extra Prompt:

Check whether this journal contains:

- Self-harm indicators
- Severe depression indicators
- Crisis language
- Panic attack symptoms

Return:

risk_level:
low/medium/high

reason:

If High:

Show:

It sounds like you're experiencing intense distress.

Please consider reaching out to:
- Trusted family member
- Friend
- Counselor
- Mental health professional

Judges love responsible AI.

UI Pages
Home
Today's Mood
Daily Journal
Quick Check-in
AI Insights
Stress Level: 8/10

Top Trigger:
Mock Tests

Confidence:
Low
Wellness Actions
3 Minute Breathing

Focus Reset

Sleep Reminder

Motivation Boost
Weekly Report
Emotion Trend Graph

Stress Trend

Top Triggers

AI Recommendations
Gemini Prompt for Motivation
Student Profile:

Exam: JEE
Stress: High
Confidence: Low

Generate:

1 motivational message.

Keep it:
- Human
- Encouraging
- Non-generic
- Maximum 80 words.