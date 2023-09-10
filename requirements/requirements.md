Steps
=====

To commemorate World Health Day, the school organized a week-long campaign "Move!".
Every participant of the campaign had to register online,
specifying their class category and step length, and then input the number of steps taken each day of the week.

Write a program that would provide a list of the total distance
covered by all students participating in the campaign for each class category.

# Initial Data

Data is provided as **standard input** (keyboard) in the following format:

 * The first line contains the number of students who participated in the campaign _m_ (10 ≤ _m_ ≤ 50).
 * Subsequent lines contain the data of the participating students:
    * class category;
    * step length in **centimeters**;
    * the number of steps taken each day of the campaign week. 

If a student did not input the number of steps taken on a particular day, the value is 0.
Data is separated by a single space.
There was at least one student who entered the number of steps for every day of the campaign week.

# Expected Results

Present the results as **standard output** (print to the screen):

* Output a list of the total distance covered by students in each class category:
   * class category;
   * the number of students who entered steps for every day of the campaign week;
   * the total distance covered by the specified class category in **kilometers**, rounded to two decimal places.

If a participant did not input the number of steps taken on at least one day, their data is not used in the calculations.
Data is separated by a single space.

* One line should contain the data for one class category.

If there wasn't a single student in any class category who entered the number of steps every day of the campaign week,
then data for that class category does not need to be provided.
The list should be presented in the order as they were specified in the initial data file.

# Recommendations

Have a function that calculates:
 * the total distance covered in kilometers for each class category
 * and counts how many students of that class category entered the number of steps taken every day of the campaign week.

# Example Input

```
10
7 76 4353 8738 4946 6484 8946 6336 6284
11 74 4352 4578 7239 3157 7856 4648 5850
6 70 5731 9017 7641 6785 8865 3184 6800
5 68 9147 9702 8671 0 5398 9555 7141
8 71 7550 0 9089 8446 4390 0 7901
7 68 4227 7160 9565 3297 4401 5740 6908
7 73 6362 6705 0 9017 5971 3154 3585
6 73 7053 8752 7606 4079 5204 3819 3310
5 73 4263 5836 3336 5401 4719 0 0
8 71 8588 5617 6903 9565 6445 6786 4522
```

Where
 * First line (`10`): number of students who participated in the campaign
 * Following lines (`7 76 4353 8738 4946 6484 8946 6336 6284`): class category, step length in _cm_, number of steps taken each day of the campaign week
 * Value `0` means that the student did not enter the number of steps taken on that day

# Example Output

```
7 2 63.11
11 1 27.88
6 2 62.69
8 1 34.38
```

Where for each line:
 * First value (`7`): class category
 * Second value (`2`): number of students who entered the number of steps taken every day of the campaign week
 * Third value (`63.11`): total distance covered in kilometers