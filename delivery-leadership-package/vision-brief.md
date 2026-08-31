# Evergreen Quote: Vision Brief

> Copy this file into `delivery-leadership-package/vision-brief.md` in your repo and fill it in. Target length: 1 page (~300 words). Write for a Liberty Mutual VP who has 90 seconds.

## Product
**Name:** Evergreen Insurance Quote (Phase 2 React rebuild)
**Delivery week:** 2
**Delivery Lead:** Tina Matthys
**Engineering team (represented by):** https://github.com/asc1-student15/wa3859-cap-phase-2-capstone-project-leaders
**GitHub Project board:** 

## Who is the customer?
The customer is a first time insurance buyer who does not have the patience to wait for a quote or push many buttons. If they don't get a believable quote within a few clicks, they will take their business elsewhere.

## What pain does Evergreen Quote remove?
Today the site has too many clicks. It requires pressing the submit button and updating the page to see the most recent quote. This update removes the click and updates the quote in real time without the extra click.

## What does "good" look like at end of the week?
- The estimate updates live as the visitor types; auto, home, and life all
  return believable numbers under the sponsor's rate decision.
- Recent quotes load from the data feed with a visible loading state, and a
  saved quote appears at the top of the list instantly.
- Work is merged to main and presentable

## What are we explicitly NOT doing this week?
- No real rate engine or actuarial pricing; the rate model is a placeholder.
- No customer accounts, saved-quote persistence, or email capture.
- No payment, checkout, or policy purchase.
- No back-end service; the JSON data feed *represents* the quotes API.
- No routing, no test suite, no deployment; Phase 2 stops at a green build.

## How will we know if it worked?
- All parts of the page should render upon load
- The customer should be able to enter a minimal amount of information and get an instant quote
- The quote provided should be based on the rating algorithm coded
- The quote should be updated instantly if any new data is entered or changed
