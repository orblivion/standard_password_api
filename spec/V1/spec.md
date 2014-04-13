Format: Json
Protocol: HTTPS
Root URL: /standard_pasword_api/V1/

**Info** /

Accepts:
    GET HEAD

Input:
    (none)

Returns:
    info: ""

Change Password /change_password/

Accepts:
    POST

Input:
    old_password: <string>
    new_password: <string>

Output:
    success: "true"|"false"
    error: "authentication"|"password_format"
    password_specifications: <string>
        * Ex - "Password should have at least 8 characters, including one digit and one symbol."
        * Free form
        * Complete sentence.
        * Useful for a user dialog
