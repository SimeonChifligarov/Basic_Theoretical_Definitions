# TODO Update this one...


# API
 - API stands for application programming interface,
which is a set of definitions and protocols for building and integrating application software.

 - a software intermediary that allows two applications to talk to each other.
Each time you use an app like Facebook, send an instant message, or check the weather on your phone, you're using an API.

 - An API is essentially a set of rules that dictate how two machines talk to each other.
Some examples of API-based interactions include a cloud application communicating with a server,
servers pinging each other, or applications interacting with an operating system.

 - It's a communications mechanism that allows applications to communicate.
 - Loosely defined, API describes everything an application programmer needs to know about piece of code to know how to use it.

========================================================================

# ASCII
 - American Standard Code for Information Interchange, a standard data-encoding format for electronic communication between computers.
ASCII assigns standard numeric values to letters, numerals, punctuation marks, and other characters used in computers.
 - It is a code for representing 128 English characters as numbers, with each letter assigned a number from 0 to 127.
For example, the ASCII code for uppercase M is 77.
Most computers use ASCII codes to represent text, which makes it possible to transfer data from one computer to another.


# UUID
 - A UUID (Universal Unique Identifier) is a 128-bit value used to uniquely identify an object or entity on the internet.
Depending on the specific mechanisms used, a UUID is either guaranteed to be different or is, at least,
extremely likely to be different from any other UUID generated until A.D. 3400.

 - Универсален уникален идентификатор е 128-битов етикет, използван за информация в компютърните системи.
Използва се и терминът глобално уникален идентификатор. Когато се генерират съгласно стандартните методи,
UUID са уникални за практически цели.

========================================================================

# urlpatters variable (Django urls.py)
 - Default Path Converters
    - str – matches any non-empty string, excluding "/"
    - int – matches zero or any positive integer
    - slug – matches any slug string consisting of ASCII letters, numbers, hyphen and underscore characters
    - path - matches any non-empty string, including "/"
      - Allows you to match a complete URL path
    - uuid – matches a formatted UUID

========================================================================

# Django Template Language
 # csrf_token Tag
   - Cross-site Request Forgery protection
   - Used inside the <form> element
   - Cross-site request forgeries:
      - type of malicious exploit 
      - unauthorized commands are performed on behalf of an authenticated users
   - More about Cross-site Request Forgery - https://www.squarefree.com/securitytips/web-developers.html#CSRF

# Template Tags Helper Functions
 - Django provides us with helper functions that allow us to create our custom template tags
    - simple_tag - processes the data and returns a string
    - inclusion_tag - processes the data and returns a rendered template
    - assignment_tag - processes the data and sets a variable in the context

# Template Inheritance
 - Template inheritance allows us to build a base skeleton template
 - The base template contains all the common elements and defines blocks that child templates can override
 - Typically, header, footer etc. remain the same in the whole app
 - Using template inheritance, we can reuse the common parts of our app

### Using include in templates
 - We can also use the include tag to include an existing template
 - {% include "blog_header.html" %}


# Django Validators
 - EmailValidator
 - URLValidator
 - MinValueValidator / MaxValueValidator
 - MinLengthValidator / MaxLengthValidator
 - RegexValidator
