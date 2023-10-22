---
layout: post
title: "Python - 5 standard library features that you should know"
date: 2023-10-22 09:00:00 +1100
categories: stuff
tags: python, data


---
The Python Standard Library provides a wealth of modules and functions to handle many common tasks without needing to install any external libraries. 

Here are five useful features:

1. **json**: This module can parse JSON from strings or files. The module can also convert Python dictionaries into JSON strings. This is especially useful in web applications, RESTful APIs, or for data storage and communication.

    Example:
    ```python
    import json

    # Convert a Python dictionary to a JSON string
    json_string = json.dumps({"name": "John", "age": 30})

    # Parse a JSON string to a Python dictionary
    parsed_json = json.loads(json_string)
    ```

2. **datetime**: This module supplies classes for manipulating dates and times in both simple and complex ways. You can handle timezones, arithmetic operations on datetime objects, formatting, and more.

    Example:
    ```python
    from datetime import datetime

    # Get the current date and time
    now = datetime.now()

    # Format a date
    formatted_date = now.strftime("%Y-%m-%d %H:%M:%S")
    ```

3. **os and os.path**: These modules provide a portable way of using operating system-dependent functionality like reading or writing to the file system, creating directories, or fetching environment variables.

    Example:
    ```python
    import os

    # Get the current working directory
    cwd = os.getcwd()

    # Check if a path is an existing file
    is_file = os.path.isfile("example.txt")
    ```

4. **re**: This module provides regular expression matching operations. You can use it for checking string patterns, parsing, substitution, and more.

    Example:
    ```python
    import re

    # Search for a pattern in a string
    match = re.search(r"\d+", "The answer is 42.")
    if match:
        print("Found number:", match.group())
    ```

5. **urllib**: This collection of modules helps in opening URLs (mostly HTTP) in a complex world — basic and digest authentication, redirections, cookies, and more. The `urllib.request` module specifically is used for opening and reading URLs.

    Example:
    ```python
    from urllib import request

    # Make a request to a web page
    with request.urlopen('http://example.com/') as response:
        html = response.read()
    ```

These features demonstrate the versatility of Python for a range of applications, from web and Internet development, data processing, working with dates and times, regular expressions, and working with operating systems.


## Links
