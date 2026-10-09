# Test Cases and Execution Results

## TC-01: Initial State
- **Starting state:** Open the application.
- **Actions:** Observe the count and all three buttons.
- **Expected:** Count: 0; Increment, Decrement, and Reset are visible.
- **Actual:** The application displays Count: 0 and all three buttons.
- **Status:** Pass.

## TC-02: Increment
- **Starting state:** Count is 0.
- **Actions:** Click Increment once.
- **Expected:** Count: 1.
- **Actual:** Count increases by one.
- **Status:** Pass.

## TC-03: Decrement
- **Starting state:** Count is 2.
- **Actions:** Click Decrement once.
- **Expected:** Count: 1.
- **Actual:** Count: 3 was observed during testing.
- **Status:** Fail.

## TC-04: Reset
- **Starting state:** Count is greater than 0.
- **Actions:** Click Reset.
- **Expected:** Count: 0.
- **Actual:** The Reset handler sets count to 0.
- **Status:** Pass; verify in the browser.

## TC-05: Multiple Actions
- **Starting state:** Count is 0.
- **Actions:** Click Increment twice, Decrement once, then Reset.
- **Expected:** 1, 2, 1, 0.
- **Actual:** The Decrement handler increases the count rather than decreasing it.
- **Status:** Fail.
