# Example: a rough idea, one revision, then the result

The user runs a small online plant shop. They type four words and never write the prompt themselves.

**User:** lfg welcome email new customers

**lfg:**

**Read as:** A welcome email sent automatically to people who just placed their first order.
**Target:** Sonnet · **Missing (assumed):** an online shop, friendly tone, under 120 words, no discount

````markdown
## Role
You are an email copywriter for a small online shop selling houseplants.

## Task
Write the welcome email a customer receives right after their first order.

## Requirements
- Under 120 words, including the subject line
- Tone: warm and plain, like a note from the owner, not a brand
- Say what happens next (packing, delivery, a care card in the box)
- One clear link to the plant-care guide

## Constraints
- Do NOT use: "valued customer", "journey", "elevate"
- No exclamation marks in the subject line

## Output Format
**Subject:** one line
**Body:** 3 short paragraphs, then a one-line sign-off

## Success Criteria
A new customer knows what happens next and feels they bought from a person, not a warehouse.
````

Send it? (`ok` to run, or tell me what to change.)

**User:** add a 10% code for their next order, code LEAF10

**lfg:** *(revises only what changed)*

**Read as:** The same welcome email, now with a 10% code for the next order.
**Target:** Sonnet · **Missing (assumed):** the code has no expiry date

````markdown
## Requirements
- Under 120 words, including the subject line
- Tone: warm and plain, like a note from the owner, not a brand
- Say what happens next (packing, delivery, a care card in the box)
- One clear link to the plant-care guide
- End with the code "LEAF10" for 10% off their next order, in one sentence
````

*(The other sections are unchanged.)* Send it? (`ok` to run, or tell me what to change.)

**User:** ok

**lfg:** *(runs the prompt)*

> **Subject:** Your plants are on their way
>
> Hi Sam,
>
> Thanks for your first order. We're packing it by hand today, and it should reach you in two to three days.
>
> Inside the box you'll find a small care card for each plant. For more detail, the care guide is here: [plant-care guide].
>
> If anything arrives looking unhappy, reply to this email and we'll sort it out. As a thank-you, use LEAF10 for 10% off your next order.
>
> Ana, Leaf & Co

*(The user approved twice and typed 13 words in total. The prompt did the rest.)*
