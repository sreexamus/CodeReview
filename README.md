# CodeReview

Reviewing Pull Requests has become day to day practice of all the developers.
Its important to know what are all the basic points to look for while reviewing PR's
Swift, SwiftUI related code rules that we need to check while reviewing

1. remove use of self where ever unnecessary. use it only in closures where its need to access instance properties.
2. Use Final Keyword for Class to make it submost class. It improves performance of the class as the compiler knows it doesn't have any subclass and need to look
   for variables, methods overridings.
3. use let for variables instead of var unless your mutating it.
4. use struct for models not classes.
5. use private for variables, functions unless your testing them
6. move all the business logic to viewmodels than in Views for better testing.
7. use reserveCapacity for the arrays when you know definite number of elements will be added.
