# Error

Use the Error API to interrogate the results of thrown errors or errors that are
returned as part of the asynchronous function calls. This module is available
without an explicit `require('error')`.

Examples:

    try {
        Integer.parseInt('string');
    } catch (error) {
        
        // English text message describing the failure that occurred
        error.errorMessage;

        // Message ID in hex string format
        error.errorCode;

        // English help text describing what the error is and the cause.
        error.errorDescription; 

        // English suggestion on how to resolve the error
        error.errorSuggestion;

        // Back trace listing the call stack leading up to the error occurrence.
        error.stack;
        
        session.output.write(error);
    }
 