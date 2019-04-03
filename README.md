This is a very simple Flask app that lets you identify & get the spans of text that are the names of popular Python packages.

The app is currently served on App Engine at https://api-test-project-236423.appspot.com/. 

To query it, you can use the following Python syntax:

```
import requests
input_text  = "Pandas is my favorite library. I don't like numpy as much as future."
requests.post('https://api-test-project-236423.appspot.com/api', json=input_text).json()
```
