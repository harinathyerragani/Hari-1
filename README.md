**GainDietPlan**

## Overview:

The GainDietPlan smart contract helps users manage a structured diet plan aimed at increasing body weight over a set period. It provides functions to set initial body weight, monitor daily calorie intake, and track missed days from the plan.

## Usage:

1. **Setting Initial Body Weight:**
   - Function: `calorieIntake(uint256 _initialWeight, uint256 _dailyCalories)`
   - Description: Allows users to set their initial body weight and daily calorie intake goal.
   - Constraints:
     - Initial weight must exceed 40 kg.
     - Daily calorie intake must be above 2000.

2. **Tracking Missed Days:**
   - Function: `missedDays(uint256 _daysMissed)`
   - Description: Updates the total missed days from the diet plan.
   - Behavior:
     - Reverts if more than 5 consecutive days are missed.

## Smart Contract Details:

- **Public State Variables:**
  - `initialBodyWeight`: Stores the initial body weight.
  - `totalMissedDays`: Tracks the total missed days.

- **Private State Variable:**
  - `currentBodyWeight`: Stores the current body weight (not directly accessible).

## License:

This smart contract is licensed under the MIT License. Please refer to the SPDX-License-Identifier tag for details.

## Author 
Harinath

harinathyerragani@gmail.com
