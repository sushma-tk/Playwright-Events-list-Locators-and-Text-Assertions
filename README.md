# Playwright EventHub – Events List Locators & Text Assertions

## Overview

This project tests the Events page of [EventHub](https://eventhub.rahulshettyacademy.com) using Playwright. It covers filtering events, extracting text from event cards, opening the correct event detail page, and comparing cards in the list, all without hard waits.

## What's covered

- **Login:** signs in and opens the Events page from Browse Events
- **Filters:** searches for `World`, selects category `Conference` and city `Hyderabad`, using different locator strategies
- **Card checks:** narrows the list to the `World Tech Summit` card and confirms exactly one match
- **Text extraction:** captures the title, price and seats from that card, then verifies the title, that the price contains `$`, and that the seat count is greater than 0
- **Scoped click:** opens Book Now from inside the matching card only
- **Detail page:** confirms the URL contains `/events/` and the heading and price match the captured values
- **List comparison:** clears the filters, confirms at least 3 cards, and checks that the first, second and last titles are non-empty and that the first and last titles differ

## To run the tests

```bash
npx playwright test
```
