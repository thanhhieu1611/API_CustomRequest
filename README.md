# API_CustomRequest
This project using API custom RequestQueue as a singleton
If you just need to make a one-time request and don't want to leave the thread pool around, 
you can create the RequestQueue wherever you need it and call stop() on the RequestQueue 
once your response or error has come back, using the Volley.newRequestQueue() method 
described in Sending a Simple Request. But the more common use case is to create 
the RequestQueue as a singleton to keep it running for the lifetime of your app. 
