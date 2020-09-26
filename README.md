# RUNNING FUNCTIONS THROUGH TERMINAL

## Use a package.json to configure yours scripts

1. In this example I used the script "example_function" to illustrate the call to a simple function inside a .js file.
  in the package.json:

    "example_function": "run-func services.js exampleFunction"

  the script consists of three parts:
    * call from the run-func library.
    * path of the .js file.
    * function name.

  in a terminal:

    >yarn example_function 
      
    or

    >npm run example_function

  When running the scrpit in the terminal we get the expected return:

    "this function is running script through of terminal command line"

2. In second example I running a script "example_function_with_param" to calling a function with param.

  in the package.json:

    "example_function_with_param": "run-func services.js exampleFunctionWithParam"
  
  in a terminal:

    >yarn example_function_with_param param1
      
    or

    >npm run example_function_with_param param1
  
  In this case I used param to display the content variable in the output string using template literals.

    "this function is running script through of terminal command line with param 'param1'"

