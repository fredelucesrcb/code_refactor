# code_refactor

The code is scalable and shows separation of concerns and will provide scalability and rapid integration due to the application of the repository method. Because of this, 
implementaion of newer technologies will be easier should the need arise in the future. Testing will also be easier since the the business logic is decoupled with the controller.

Some of the problems I have encountered with the code are the following:
  1. initiating of empty arrays as array() = since PHP 5.4, the shorthand declaration of arrays as [] has been available. Maybe it's just a matter of personal preference,
      but I seem to like the shorthand declaration as it is cleaner compared to the traditional way of declaring empty arrays. Though if the application needs backward compatibility,
      I would stick with the old way of declaring empty arrays,
  2. using == instead of === in comparison operators - in order to make the app more robust and less prone to bugs and data type errors, it is best to use the === or !== operators.
     It is also sightly less taxing to the speed of the application to use the === comparison operators since the operator does not unecessarily converts the values into other possible
     data types.
  3. repetitive code that can be found in multiple methods.
  4. Implicit If-else statements that could cause errors and afect the code's readability.
  
  If I were to redesign the code from scratch, I would rely heavilly on helper functions, even using traits and place the query builder code into another file so that it can be dynamically
  used by another part of the app.
