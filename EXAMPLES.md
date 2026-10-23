# Examples

Before/after examples, one per rule.

## 1. Close every gap before you start

**Request:** "Build an admin page"

**❌** Builds login, a user list, and charts on a guess.

**✅**
```
One question before I start. What is the first job this page must do?
A. Look up and block users (recommended: it's what you need when something goes wrong)
B. View revenue and signup numbers
C. Approve or remove content
```

If the user says "all of them", ask again: "I need one to build first so the order is clear. Start with A and queue the rest?"

## 2. Fix the part, keep the whole

**Request:** "Change 'credits' to 'points' in this section"

**❌** Changes that section only. The other 12 places still say "credits", so the product now uses two words for one thing.

**✅**
```
"Credits" is the product-wide term (12 places). Changing one section mixes the terms.
A. Keep "credits" here and just reword the sentence (recommended: keeps the decided term)
B. Rename the term to "points" everywhere, all 12 places
```

## 3. Complexity is a budget

**Situation:** A "skip duplicates within 5 seconds" rule was added to stop duplicate notifications. Duplicates still arrive.

**❌** Raises the window to 10 seconds and adds another exception.

**✅**
```
Second failed fix on the same problem, so I stopped.
Original problem: one notification arrives twice.
Current state: two skip rules stacked, duplicates unchanged.
Premise I was assuming: duplicates come from the sender. Testing it: two workers pick up the same job.
Proposal: remove both skip rules and lock the job so one worker takes it.
```

## 4. One correction means a pattern

**Request:** "The save button is cut off on mobile on the settings page"

**❌** Fixes the settings page only.

**✅**
```
Principle: buttons must fit a 375px screen. Cause: fixed width in the shared button style.
Checked all 14 pages at 375px. Same issue on settings, profile, billing, invite.
Fixed the shared style once; all four pass. Added a 375px screenshot test.

Other problem, reported only: the card number field doesn't open the numeric keypad on iOS.
```

## 5. Done means verified

**Request:** "Is it done?"

**❌** "Yes, login works."

**✅**
```
Verified: email login passed 3 times in the browser; session survives a reload.
Not verified: Google login. No OAuth key locally.
Remaining: Google login check.
```

## Conversation

**Request:** "Why does this error happen?"

**❌** "The client is instantiated prior to environment variable resolution, causing a configuration race."

**✅** "The database connection is created before the settings file is read. Swapping the order fixes it. Want me to?"

## Code

**Request:** "Add coupon discounts to checkout"

**❌** Adds an `if (coupon)` branch inside checkout and copies the same math into the order screen. The discount now lives in two places.

**✅**
```
Price calculation has one owner: the pricing module. I added coupons as a rule there.
Checkout and the order screen only read the result.
The next discount type (store credit) goes in the same place.
```
