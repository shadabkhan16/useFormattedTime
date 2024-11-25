# useFormattedTime

A React hook to format and dynamically update remaining time in human-readable units (days, hours, minutes).

## Installation

```bash
npm install use-formatted-time
```

# Parameters

initialMinutes (number): The initial time in minutes.

# Returns

(string): A string representing the formatted time left, e.g., "1 day 1 hr" or "45 mins".

# Usage

Here’s an example of how to use the hook:

```
import useFormattedTime from "use-formatted-time";

const Timer = () => {
  const formattedTime = useFormattedTime(1500); // 1500 minutes = 1 day 1 hr

  return <p>Time Remaining: {formattedTime}</p>;
};

export default Timer;

```

# Features

1. Automatically decrements the remaining time by 1 minute every minute.
2. Formats time intelligently into days, hours, and minutes.
3. Stops at 0 minutes to avoid negative values.

# License

This package is licensed under the MIT License.
