# Java Leap Year Checker

A small Java console program that reads a year and tells whether it is a leap year.

## Leap Year Rules

A year is a leap year if:

- it is divisible by **400**, or
- it is divisible by **4** but **not** by **100**

```java
if (year % 400 == 0 || (year % 4 == 0 && year % 100 != 0)) {
    System.out.println(year + " is a Leap Year");
} else {
    System.out.println(year + " is not a Leap Year");
}
```

## Examples

| Year | Result | Why |
|------|--------|-----|
| 2024 | Leap Year | Divisible by 4, not by 100 |
| 2023 | Not a Leap Year | Not divisible by 4 |
| 1900 | Not a Leap Year | Divisible by 100 but not by 400 |
| 2000 | Leap Year | Divisible by 400 |

## Sample Run

```
Enter a year: 2024
2024 is a Leap Year
```

## Requirements

- Java Development Kit (JDK) 8 or higher

## Getting Started

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
javac LeapYear.java
java LeapYear
```

## Notes

- Entering something that is not a whole number throws an `InputMismatchException`.

## Project Structure

```
.
├── LeapYear.java
└── README.md
```

## Possible Improvements

- Handle invalid input with `hasNextInt()` or `try-catch`
- Move the check into a method such as `isLeapYear(int year)`
- Print all the leap years in a range
