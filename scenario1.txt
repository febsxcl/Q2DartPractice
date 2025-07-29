void main() {
  // Subject scores
  double filipino = 79.9;
  double math = 86.5;
  double science = 84.3;

  // Compute average
  double finalAverage = (filipino + math + science) / 3;

  // Determine pass/fail
  String result = finalAverage >= 60 ? 'PASSED!!' : 'FAILED!!';

  // Determine grade equivalent
  String gradeLetter;
  if (finalAverage >= 90) {
    gradeLetter = 'A';
  } else if (finalAverage >= 80) {
    gradeLetter = 'B';
  } else if (finalAverage >= 70) {
    gradeLetter = 'C';
  } else if (finalAverage >= 60) {
    gradeLetter = 'D';
  } else {
    gradeLetter = 'F';
  }

  // Output
  print('Filipino Grade: $filipino');
  print('Math Grade: $math');
  print('Science Grade: $science');
  print('Final Average: ${finalAverage.toStringAsFixed(2)}');
  print('Result: $result');
  print('Grade Equivalent: $gradeLetter');
}
