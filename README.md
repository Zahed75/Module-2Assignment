# Module-2Assignment

```
You are building a student grading system. Each student has a name and a test score. Your task is to write a Dart function called studentGrade that takes in the student's name and test score, and returns their corresponding grade based on the following grading scale:
A: 90 - 100
B: 80 - 89
C: 70 - 79
D: 60 - 69
F: 0 - 59

The function should validate the test score and ensure it is within the valid range of 0 to 100. If the score is valid, it should return the grade. If the score is invalid, it should return "Invalid Grade".

Here's an example usage of the studentGrade function:

void main() {
  String studentName = "Saiaf Anan";  /// student name must be yours
  int testScore = 85;
  String grade = studentGrade(studentName, testScore);
  print("$studentName's grade: $grade");


}


In this example, the studentGrade function should check the test score of your full name and assign the corresponding grade based on the grading scale. Since you scored 85, it falls within the range of 80-89, so the function should return "B".
```


<b>solution</b>

```
String studentGrade(String name, int score) {
  if (score < 0 || score > 100) {
    return "Invalid Grade";
  } else if (score >= 90) {
    return "A";
  } else if (score >= 80) {
    return "B";
  } else if (score >= 70) {
    return "C";
  } else if (score >= 60) {
    return "D";
  } else {
    return "F";
  }
}

void main() {
  String studentName = "Saiaf Anan";
  int testScore = 85;
  String grade = studentGrade(studentName, testScore);
  print("$studentName's grade: $grade");
}

```