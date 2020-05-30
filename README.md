# Response Formatter
This library will help you to work with flask application without hesitating responses and exception in routes.

#### How to use
    
    1)  To get exceptions as response messages use like below. Make sure to set 'allow_exception=False'.
        Once you done you would be able work without breaking when exception comes. The exception will come
        as a response
    
        @app.route('/')
        @response_format(allow_exception=False)
        def hello_world():
            return {}, True, 200, 'message'
    
    2) For see the exceptions. Onec you give 'allow_exception=True' it will allows to raise the exception and
       the app would breake as usual way.
    
       @app.route('/')
       @response_format(allow_exception=True)
       def hello_world():
           return {}, True, 200, 'message'
 
                 